# Upload Server

In terms of type `pv`, `nfs` and `hostpath` volume, we can use `Upload Server` feature that allows users to upload files to a volume.

**Editing** a created type `pv`, `nfs` and `hostpath` volume, we should see `Enable Upload Server` toggle and `Regenerate Secret` button.

<figure><img src="../../.gitbook/assets/dataset_pv_v2_upload_server.png" alt=""><figcaption></figcaption></figure>

Toggle `Enable Upload Server` on, and click `Confirm`. There is a pop-up showing the credential (`Username` / `Password`) for the uploader access.

<figure><img src="../../.gitbook/assets/dataset_pv_v2_credential.png" alt=""><figcaption></figcaption></figure>

Since the credential shows once only, you **must** keep it in a memo before clicking `OK`.

**Note: if credential is lost** you can go back to volume editing page and click `Regenerate Secret` button again to have a new pair of credential.

You can see a `Link` created in `Upload Server` field of the volume.

<figure><img src="../../.gitbook/assets/dataset_pv_v2_upload_server_enable.png" alt=""><figcaption></figcaption></figure>

Clicking the link, and input the credential you keep in the memo.

<figure><img src="../../.gitbook/assets/dataset_pv_v2_upload_server_login2.png" alt=""><figcaption></figcaption></figure>

After login the upload server, it displays a file list and click `Upload Data`.

<figure><img src="../../.gitbook/assets/dataset_pv_v2_file_manager_upload.png" alt=""><figcaption></figcaption></figure>

A upload dialogue appears.

<figure><img src="../../.gitbook/assets/dataset_pv_v2_upload_dialogue.png" alt=""><figcaption></figcaption></figure>

Dragging files for uploading, files are not uploaded yet at this moment.

{% hint style="info" %}
Uploader supports **auto-unzip** to a zip file. Dragging a **zip** file in, the file will be **unzip automatically** and the directory structure is remained.
{% endhint %}

Click `Upload n files` to trigger the upload. It shows **Complete** at bottom of the uploader once finished.

Close the uploader and back to the file list, uploaded files are listed.

<figure><img src="../../.gitbook/assets/dataset_pv_v2_upload_button.png" alt=""><figcaption></figcaption></figure>

You can find these uploaded files in the volume which is mounted on the hub in your jupyter notebook. Currently these files can be removed only via notebook.

<figure><img src="../../.gitbook/assets/dataset_pv_v2_file_uploaded.png" alt=""><figcaption></figcaption></figure>
