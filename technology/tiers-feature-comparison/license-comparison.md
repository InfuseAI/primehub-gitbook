# License Comparison

In addition to feature differences among tiers, some features are also varied in licenses.

* EE Trial: Enterprise Edition with Default License.
* EE Licensed: Enterprise Edition with Authorized License.
* Deploy Trial: Deploy Edition with Default License.
* Deploy Licensed: Deploy Edition with Authorized License.

Here we list the features comparison among licenses.

| Features                  | EE Trial                      | EE Licensed               | Deploy Trial                  | Deploy Licensed           |
| ------------------------- | ----------------------------- | ------------------------- | ----------------------------- | ------------------------- |
| Kubernetes Nodes          | Maximum: 1 node               | Depends on License Detail | Maximum: 1 node               | Depends on License Detail |
| Admin > Users Management  | Maximum: 5 users              | Depends on License Detail | Maximum: 5 users              | Depends on License Detail |
| Admin > Groups Management | Maximum: 1 group              | Depends on License Detail | Maximum: 1 group              | Depends on License Detail |
| Deployments               | Maximum: 1 deployment running | Depends on License Detail | Maximum: 1 deployment running | Depends on License Detail |

***

### FAQ

**Q: What is the license detail?**

* For each license, we determine the:
  * \# of nodes allowed
  * \# of users allowed
  * \# of groups allowed
  * \# of deployments allowed
  * License Start Time
  * License Expiration Time

**Q: What is the default license?**

* When we install a PrimeHub EE or PrimeHub Deploy, there is a default license installed.
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

*   The console would show a warning message:

    > You are using more nodes than your license allows. Please contact your system administrator.

**Q: What happens if I upgrade from CE to EE, and the # of users/groups exceeds the limitation in license?**

* The existing users/groups would not be affected, but it is not allowed to create new user/group.
