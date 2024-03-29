# Persistence

PrimeHub provides several types of persistent data stores. This document describes the characteristics of each of them, and the conditions in which they perform the best.

## Volume Types

### User Volume

A user's private storage.

A User Volume is **good** for:

* Storing personal data. (e.g. datasets, code)

A User Volume has the following **limitations**:

* It can only be accessed via notebooks.

### Shared Volume

A volume shared among group members. All members can read and write data to this volume. It is like an NFS server for a group.

A Shared Volume is **good** for:

* Storing shared data among members in a group
* Exchanging data among notebooks, jobs, and apps

A Shared Volume **cannot be used** for:

* Downloading and uploading data through an API/CLI/SDK

A group's Shared Volume is not enabled by default. Please contact the system administrator to enable it. For more information, Please see [Group Management](../../administrator-guide/group-management.md).

### PHFS Storage

PHFS (PrimeHub File System) is shared among group members, like a Shared Volume. However, PHFS has the added benefit of being [object storage](https://en.wikipedia.org/wiki/Object\_storage), similar to S3. Due to the characteristics of object storage, PHFS provides the best accessibility out of all kinds of storage.

Data stored in PHFS can be found under the subpath `/groups/<group>` of an object storage bucket.

There are several ways to **access data stored in PHFS**:

* PHFS can be mounted in notebooks, apps, and jobs.
* Users can download/upload content from the [Shared Files](../../user-guide/shared-files.md) UI in the User Portal.
* Users can list and download files from the [PrimeHub SDK/CLI](https://github.com/infuseai/primehub-python-sdk).

PHFS is **good** for:

* Uploading and downloading files via the Shared Files UI
* Data exchange through [PrimeHub SDK/CLI](https://github.com/infuseai/primehub-python-sdk)
* Storing the [artifacts](../../user-guide/jobs-recurring-jobs/job-artifacts.md) of a job's output
* The source of model files for model deployment

Even though we can access the PHFS from the filesystem, the access mode is **not fully POSIX-compatible**. It does not allow _random access_ and _append write_. It's only suitable for _sequential read_ and _sequential write_ operation.

Due to this limitation PHFS **cannot be used for**:

* Uploading a file with size **> 1MB** from the notebook UI (i.e. Jupterlab upload feature). An error will occur and the uploaded file will be truncated to 1MB. **To upload files larger than 1MB, please use the \_Shared Files**\_\*\* UI.\*\*
* The output of training. Some ML frameworks cannot output training results successfully to PHFS. For example, in TensorFlow, writing model files in _HDF5_ format to PHFS will cause the error `Problems closing file (file write failed: ...)` due to _HDF5_ using _seek_ while writing. **To store training results in PHFS, first output to a User Volume or Shared Volume, and then copy to PHFS.**
* The input of training. PHFS has the worst performance out of all kinds of storage. **To train a dataset multiple runs, we recommend putting them in user volume or group volume.**

PHFS is not installed by default, please check this document to [configure PrimeHub store and PHFS](../../technology/concept/broken-reference/).

### Data Volume

A Data Volume is a storage type that can be shared among multiple groups. The following permission settings can be configured:

* Read-only on a global or per-group basis
* Writable on a per-group basis

There are **several kinds** of Data Volumes we can create:

* **Persistent volume (PV)**: Like group volume, but can be shared among multiple groups rather than just a single group.
* **NFS**: A volume that connects to an external NFS server.
* **Host Path**: A special kind of volume that mounts the host filesystem.
* **Git**: A special kind of volume which syncs the upstream git repository periodically. The actual data is stored on the host filesystem.
* **Env**: Technically, this is not a volume, but a method to configure environment variables to be used in notebooks and jobs.

A Data Volume is **good** for:

* Sharing among groups. In an education environment, for example, datasets could be shared among multiple teams (groups) of students with read-only permissions, while the teaching assistants could be in another group with write permissions.
* Special storage destination (e.g. external NFS server, host path, git sync)

A Data Volume has the following **limitations**:

* Data cannot downloaded and uploaded through API/CLI/SDK
* If the volume is to be used by only one group then, due to its ease of use, a Shared Volume is preferred

A Data Volume is configured by the system administrator. For more information, Please see [Volume Management](../../administrator-guide/volume-management/). In some types of the volume, we can also configure a [upload server ](../../administrator-guide/volume-management/upload-server.md)to upload data to the data volume.

## Comparison

| Type         | Shared by                | API/UI Access | Use case                 |
| ------------ | ------------------------ | ------------- | ------------------------ |
| User Volume  | No                       | No            | Private data             |
| Group Volume | Group members of a group | No            | Shared data in group     |
| PHFS         | Group members of a group | Yes           | Data import/export       |
| Data Volume  | Multiple groups          | No            | Shared data among groups |

All four storage options can be accessed via the file system. The following table describes the mount points and characteristics:

| Type         | Available in                     | Mount point          | Characteristic                                                               |
| ------------ | -------------------------------- | -------------------- | ---------------------------------------------------------------------------- |
| User Volume  | Notebooks                        | `/home/jovyan`       | <p>Best performance<br>(like block device)</p>                               |
| Group Volume | <p>Notebooks<br>Apps<br>Jobs</p> | `/project/<group>`   | <p>Good performance<br>(like NFS)</p>                                        |
| PHFS         | <p>Notebooks<br>Apps<br>Jobs</p> | `/phfs`              | <p>Limited access mode<br>Sequential Read/Write<br>(like object storage)</p> |
| Data Volume  | <p>Notebooks<br>Apps<br>Jobs</p> | `/datasets/<volume>` | <p>Good performace<br>(like NFS)</p>                                         |
