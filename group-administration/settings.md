# Settings

Enterprise Applicable to Enterprise EditionCommunity Applicable to Community EditionDeploy Applicable to Deploy Edition\


Group Admin now can view the current settings of the managed group which are configured by Platform Administrator. All of settings are viewable-only to Group Admin, except **Default Timeout Setting** of Jobs is configurable.

> To request Platform Administrator for adjustments.

### Info

It displays the current settings, **Name**, **Display Name**, **Shared Volume**, **User Quota** and **Group Quota** of the working group.

### Members

It displays group members and group administrators.

### Jobs

Enterprise Applicable to Enterprise Edition\


* `Default Timeout Setting`: Set Minutes / Hours / Days.

Group Admin can apply a group-wise Job timeout setting on every jobs submitted from the group. A running job will be cancelled when it exceeds the setting. This setting is able to be overwritten by each job submission for the customization. By default it is 7 days.

### Deployments

Enterprise Applicable to Enterprise EditionDeploy Applicable to Deploy Edition\


It displays if **Model Deployment** is enabled to the group, i.e., if the group can use **Deployments** feature.

### MLflow

Enterprise Applicable to Enterprise EditionDeploy Applicable to Deploy Edition\


PrimeHub provides Models feature by integrating with MLflow app instance. We can easily set up the MLflow app in the following steps:

1. Click `Create MLflow App` link to create the MLflow app.&#x20;
2. After the MLflow app is successfully created, we can choose it from the `Configure with Installed Apps` selector. Both the required information `MLflow Tracking URI` and `MLflow UI URI` will be automatically filled.&#x20;
3. Click `Save` button to keep the setting for binding Models to the MLflow instance.

Furthermore, if we have another installed MLflow app instance, then we can learn `App URL` and `Service Endpoint` from the installed App detail.

* Fill in `MLflow Tracking URI` with `http://`+`Service Endpoint`.
* Fill in `MLflow UI URI` with `App URL`.&#x20;

> By integrating externally-hosted MLflow server, see Configuration for the detail.
