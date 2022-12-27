---
description: Product tiers and licenses
---

# Tiers Feature Comparison

## Tiers

**PrimeHub** has three tiers: **Community**, **Enterprise**, and **Deploy**.

* **Community**: fundamental features provided to the community. See [Community Edition ⇗](https://github.com/InfuseAI/primehub) GitHub repo.
* **Enterprise**: fully complete features.
* **Deploy**: mandatory features dedicated to Model Deployment.

Here we list the features comparison among tiers.

| Features                          | Community | Enterprise | Deploy |
| --------------------------------- | --------- | ---------- | ------ |
| Notebooks                         | ✅️        | ✅️         |        |
| Jobs                              |           | ✅️         |        |
| Recurring Jobs                    |           | ✅️         |        |
| Models                            |           | ✅️         | ✅️     |
| Deployments                       |           | ✅️         | ✅️     |
| Shared Files                      | ✅️        | ✅️         | ✅️     |
| Datasets                          | ✅️        | ✅️         | ✅️     |
| Apps                              | ✅️        | ✅️         |        |
| SSH Server                        | ✅️        | ✅️         |        |
| Python SDK                        | ✅️        | ✅️         | ✅️     |
| PrimeHub Store                    | ✅️        | ✅️         | ✅️     |
| Submit Notebook as a Job          |           | ✅️         |        |
| Group Admin > Group Images        | ✅️        | ✅️         |        |
| Group Admin > Group Settings      | ✅️        | ✅️         | ✅️     |
| Admin > Users Management          | ✅️        | ✅️         | ✅️     |
| Admin > Groups Management         | ✅️        | ✅️         | ✅️     |
| Admin > Instance Types Management | ✅️        | ✅️         | ✅️     |
| Admin > Images Management         | ✅️        | ✅️         |        |
| Admin > Volumes Management        | ✅️        | ✅️         |        |
| Admin > Secrets Management        | ✅️        | ✅️         | ✅️     |
| Admin > Usage Report              |           | ✅️         |        |
| Admin > System Settings           | ✅️        | ✅️         | ✅️     |

## License

In addition to feature differences among tiers, some features are also varied in licenses.

* EE Trial: Enterprise Edition with Default License.
* EE Licensed: Enterprise Edition with Authorized License.
* Deploy Trial: Deploy Edition with Default License.
* Deploy Licensed: Deploy Edition with Authorized License.

Here we list the features comparison among licenses.

| Features                  | EE Trial                      | EE Licensed               | Deploy Licensed           |
| ------------------------- | ----------------------------- | ------------------------- | ------------------------- |
| Kubernetes Nodes          | Maximum: 1 node               | Depends on License Detail | Depends on License Detail |
| Admin > Users Management  | Maximum: 5 users              | Depends on License Detail | Depends on License Detail |
| Admin > Groups Management | Maximum: 1 group              | Depends on License Detail | Depends on License Detail |
| Deployments               | Maximum: 1 deployment running | Depends on License Detail | Depends on License Detail |

***

### License warning

A license issued by InfuseAI contains `Expiration Date`, `Maximum Nodes`, `Maximum Deployments`.

*   When a license has expired, a warning message appears.

    > Your license has expired. Please contact your sales team to extend your license.
*   When used node amount > granted node amount, a warning message appears.

    > You are using more nodes than your license allows. Please contact your system administrator.
*   when used model amount > granted model amount + 10%, a warning message appears.

    > Please contact your system administrator for assistance to upgrade your license to run more models.

To learn the current PrimeHub license information, see [PrimeHub License](broken-reference).

### FAQ

**Q: What is the license detail?**

For each license, we determine the:

* \# of nodes allowed
* \# of users allowed
* \# of groups allowed
* \# of deployments allowed
* License Start Time
* License Expiration Time

**Q: What is the default license?**

* When we install a PrimeHub EE , there is a default license installed.
* The detail of default license:
  * 1 node
  * 5 users
  * 1 group
  * 1 deployment
  * The license is never expired

**Q: What happens if the license is expired?**

* The normal user cannot create new resources for Jobs, Schedules, and Deployments.
* The existing resources would not be affected.

**Q: What happens if the # of node exceeds the limitation in license?**

The console would show a warning message:

> You are using more nodes than your license allows. Please contact your system administrator.

**Q: What happens if I upgrade from CE to EE, and the # of users/groups exceeds the limitation in license?**

The existing users/groups would not be affected, but it is not allowed to create new user/group.
