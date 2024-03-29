# Table of contents

* [Introduction](README.md)
* [Installation](install-manually.md)
* [Tiers and Licenses](tiers-feature-comparison.md)

## End-to-End Tutorial

* [1 - MLOps Introduction and Scoping the Project](end-to-end-tutorial/1-mlops-introduction-and-scoping-the-project.md)
* [2 - Train and Manage the Model](end-to-end-tutorial/2-train-and-manage-the-model.md)
* [3 - Compare, Register and Deploy the Model](end-to-end-tutorial/3-compare-register-and-deploy-the-model.md)
* [4 - Build the Web Application](end-to-end-tutorial/4-build-the-web-application.md)
* [5 - Summary](end-to-end-tutorial/5-summary.md)

## User Guide

* [User Portal](user-guide/user-portal.md)
* [Notebook](user-guide/start-notebook/README.md)
  * [Notebook Tips](user-guide/start-notebook/notebook-tips.md)
  * [Advanced Settings](user-guide/start-notebook/advanced-settings.md)
  * [PrimeHub Notebook Extension](user-guide/start-notebook/primehub-notebook-extension.md)
  * [Submit Notebook as Job](user-guide/start-notebook/submit-notebook-as-job.md)
* [Jobs](user-guide/jobs-recurring-jobs/README.md)
  * [Job Artifacts](user-guide/jobs-recurring-jobs/job-artifacts.md)
  * [Tutorial](user-guide/jobs-recurring-jobs/tutorial/README.md)
    * [(Part1) MNIST classifier training](user-guide/jobs-recurring-jobs/tutorial/part1-mnist-classifier-training.md)
    * [(Part2) MNIST classifier training](user-guide/jobs-recurring-jobs/tutorial/part2-mnist-classifier-training.md)
    * [(Advanced) Use Job Submission to Tune Hyperparameters](user-guide/jobs-recurring-jobs/tutorial/advanced-use-job-submission-to-tune-hyperparameters.md)
    * [(Advanced) Model Serving by Seldon](user-guide/jobs-recurring-jobs/tutorial/advanced-model-serving-by-seldon.md)
    * [Job Artifacts Simple Usecase](user-guide/jobs-recurring-jobs/tutorial/job-artifacts-simple-usecase.md)
* [Models](user-guide/models/README.md)
  * [Manage and Deploy Model](user-guide/models/manage-and-deploy-model.md)
  * [Model Management Configuration](user-guide/models/model-management-configuration.md)
* [Deployments](user-guide/deployments/README.md)
  * [Pre-packaged servers](user-guide/deployments/pre-packaged-servers/README.md)
    * [TensorFlow server](user-guide/deployments/pre-packaged-servers/tensorflow-server.md)
    * [PyTorch server](user-guide/deployments/pre-packaged-servers/pytorch-server.md)
    * [SKLearn server](user-guide/deployments/pre-packaged-servers/sklearn-server.md)
    * [Customize Pre-packaged Server](user-guide/deployments/pre-packaged-servers/customize-pre-packaged-server.md)
    * [Run Pre-packaged Server Locally](user-guide/deployments/pre-packaged-servers/run-pre-packaged-server-locally.md)
  * [Package from Language Wrapper](user-guide/deployments/package-from-language-wrapper/README.md)
    * [Model Image for Python](user-guide/deployments/package-from-language-wrapper/model-image-for-python.md)
    * [Model Image for R](user-guide/deployments/package-from-language-wrapper/model-image-for-r.md)
    * [Reusable Base Image](user-guide/deployments/package-from-language-wrapper/reusable-base-image.md)
  * [Prediction APIs](user-guide/deployments/prediction-apis.md)
  * [Model URI](user-guide/deployments/model-uri.md)
  * [Tutorial](user-guide/deployments/tutorial/README.md)
    * [Model by Pre-packaged Server](user-guide/deployments/tutorial/model-by-pre-packaged-server.md)
    * [Model by Pre-packaged Server (PHFS)](user-guide/deployments/tutorial/model-by-pre-packaged-server-phfs.md)
    * [Model by Image built from Language Wrapper](user-guide/deployments/tutorial/model-by-image-built-from-language-wrapper.md)
* [Shared Files](user-guide/shared-files.md)
* [Datasets](user-guide/datasets.md)
* [Apps](user-guide/apps-overview/README.md)
  * [Label Studio](user-guide/apps-overview/label-studio.md)
  * [MATLAB](user-guide/apps-overview/matlab.md)
  * [MLflow](user-guide/apps-overview/mlflow.md)
  * [Streamlit](user-guide/apps-overview/streamlit.md)
  * [Tutorial](user-guide/apps-overview/tutorial/README.md)
    * [Create Your Own App](user-guide/apps-overview/tutorial/create-your-own-app.md)
    * [Create an MLflow server](user-guide/apps-overview/tutorial/create-an-mlflow-server.md)
    * [Label Dataset by Label Studio](user-guide/apps-overview/tutorial/label-dataset-by-label-studio.md)
    * [Code Server](user-guide/apps-overview/tutorial/code-server.md)
* [Group Admin](user-guide/group-admin/README.md)
  * [Images](user-guide/group-admin/images.md)
  * [Settings](user-guide/group-admin/settings.md)
* [Generate an PrimeHub API Token](user-guide/generate-an-primehub-api-token.md)
* [Python SDK](user-guide/python-sdk.md)
* [SSH Server Feature](user-guide/ssh-server-feature/README.md)
  * [VSCode SSH Notebook Remotely](user-guide/ssh-server-feature/vscode-ssh-notebook-remotely.md)
  * [Generate SSH Key Pair](user-guide/ssh-server-feature/generate-ssh-key-pair.md)
  * [Permission Denied](user-guide/ssh-server-feature/permission-denied.md)
  * [Connection Refused](user-guide/ssh-server-feature/connection-refused.md)
* [Advanced Tutorial](user-guide/advanced/README.md)
  * [Labeling the data](user-guide/advanced/labeling-the-data.md)
  * [Notebook as a Job](user-guide/advanced/notebook-as-a-job.md)
  * [Custom build the Seldon server](user-guide/advanced/custom-build-the-seldon-server.md)
  * [PrimeHub SDK/CLI Tools](user-guide/advanced/primehub-sdk-cli-tools.md)

## Administrator Guide

* [Admin Portal](administrator-guide/admin-portal/README.md)
  * [Create User](administrator-guide/admin-portal/create-user.md)
  * [Create Group](administrator-guide/admin-portal/create-group.md)
  * [Assign Group Admin](administrator-guide/admin-portal/assign-group-admin.md)
  * [Create/Plan Instance Type](administrator-guide/admin-portal/create-plan-instance-type.md)
  * [Add InfuseAI Image](administrator-guide/admin-portal/add-infuseai-image.md)
  * [Add Image](administrator-guide/admin-portal/add-image.md)
  * [Build Image](administrator-guide/admin-portal/build-image.md)
  * [Gitsync Secret for GitHub](administrator-guide/admin-portal/gitsync-secret-for-github.md)
  * [Pull Secret for GitLab](administrator-guide/admin-portal/pull-secret-for-gitlab.md)
* [System Settings](administrator-guide/system-settings.md)
* [User Management](administrator-guide/user-management.md)
* [Group Management](administrator-guide/group-management.md)
* [Instance Type Management](administrator-guide/instance-type-management/README.md)
  * [NodeSelector](administrator-guide/instance-type-management/nodeselector.md)
  * [Toleration](administrator-guide/instance-type-management/toleration.md)
* [Image Management](administrator-guide/image-management/README.md)
  * [Custom Image Guideline](administrator-guide/image-management/custom-image-guideline.md)
* [Volume Management](administrator-guide/volume-management/README.md)
  * [Upload Server](administrator-guide/volume-management/upload-server.md)
* [Secret Management](administrator-guide/secret-management.md)
* [App Settings](administrator-guide/app-settings.md)
* [Notebooks Admin](administrator-guide/notebooks-admin.md)
* [Usage Reports](administrator-guide/usage-reports.md)

## Reference

* [Jupyter Images](reference/jupyter-images/README.md)
  * [repo2docker image](reference/jupyter-images/repo2docker-image.md)
  * [RStudio image](reference/jupyter-images/rstudio-image.md)
* [InfuseAI Images List](developer-guide/infuseai-images-list.md)
* [Roadmap](https://github.com/orgs/InfuseAI/projects/4/views/1)

## Developer Guide

* [GitHub](https://github.com/infuseAI/primehub)
* [Design](developer-guide/design/README.md)
  * [PrimeHub File System (PHFS)](developer-guide/design/primehub-file-system-phfs.md)
  * [PrimeHub Store](developer-guide/design/primehub-store.md)
  * [Log Persistence](developer-guide/design/log-persistence.md)
  * [PrimeHub Apps](developer-guide/design/primehub-apps.md)
  * [Admission](developer-guide/design/admission.md)
  * [Notebook with kernel process](developer-guide/design/notebook-with-kernel-process.md)
  * [JupyterHub](developer-guide/design/jupyterhub.md)
  * [Image Builder](developer-guide/design/image-builder.md)
  * [Volume Upload](developer-guide/design/volume-upload.md)
  * [Job Scheduler](developer-guide/design/job-scheduler.md)
  * [Job Submission](developer-guide/design/job-submission.md)
  * [Job Monitoring](developer-guide/design/job-monitoring.md)
  * [Install Helper](developer-guide/design/install-helper.md)
  * [User Portal](developer-guide/design/user-portal.md)
  * [Meta Chart](developer-guide/design/meta-chart.md)
  * [PrimeHub Usage](developer-guide/design/primehub-usage.md)
  * [Job Artifact](developer-guide/design/job-artifact.md)
  * [PrimeHub Apps](developer-guide/design/primehub-apps-1.md)
* [Concept](developer-guide/concept/README.md)
  * [Architecture](developer-guide/concept/architecture.md)
  * [Data Model](developer-guide/concept/data-model.md)
  * [CRDs](developer-guide/concept/crds.md)
  * [GraphQL](developer-guide/concept/graphql.md)
  * [Persistence Storages](developer-guide/concept/persistence-storages.md)
  * [Persistence](developer-guide/concept/persistence.md)
  * [Resources Quota](developer-guide/concept/resources-quota.md)
  * [Privilege](developer-guide/concept/privilege.md)
* [Configuration](developer-guide/configuration/README.md)
  * [How to configure PrimeHub](developer-guide/configuration/how-to-configure-primehub.md)
  * [Multiple Jupyter Notebook Kernels](developer-guide/configuration/multiple-jupyter-notebook-kernels.md)
  * [Configure SSH Server](developer-guide/configuration/configure-ssh-server.md)
  * [Configure Job Submission](developer-guide/configuration/configure-job-submission.md)
  * [Configure Custom Image Build](developer-guide/configuration/configure-custom-image-build.md)
  * [Configure Model Deployment](developer-guide/configuration/configure-model-deployment.md)
  * [Setup Self-Signed Certificate for PrimeHub](developer-guide/configuration/setup-self-signed-certificate-for-primehub.md)
  * [Chart Configuration](developer-guide/configuration/chart-configuration.md)
  * [Configure PrimeHub Store](developer-guide/configuration/configure-primehub-store.md)
* [Environment Variables](developer-guide/environment-variables.md)
