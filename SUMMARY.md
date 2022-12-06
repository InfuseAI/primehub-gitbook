# Table of contents

## Getting Started

* [🚀 One-Click Install](README.md)
* [Install Manually](getting-started/install-manually.md)
* [Quickstart](getting-started/quickstart.md)

## Technology

* [Platform Introduction](technology/platform-introduction.md)
* [Concept](technology/concept/README.md)
  * [Persistence](technology/concept/persistence.md)
  * [Resources Quota](technology/concept/resources-quota.md)
  * [Privilege](technology/concept/privilege.md)
* [Design](technology/design/README.md)
  * [PrimeHub File System (PHFS)](technology/design/primehub-file-system-phfs.md)
  * [PrimeHub Store](technology/design/primehub-store.md)
  * [Log Persistence](technology/design/log-persistence.md)
* [Tiers Feature Comparison](technology/tiers-feature-comparison/README.md)
  * [License Comparison](technology/tiers-feature-comparison/license-comparison.md)
* [User Portal](technology/user-portal/README.md)
  * [Generate an PrimeHub API Token](technology/user-portal/generate-an-primehub-api-token.md)

## End-to-End Tutorial

* [1 - MLOps Introduction and Scoping the Project](end-to-end-tutorial/1-mlops-introduction-and-scoping-the-project.md)
* [2 - Train and Manage the Model](end-to-end-tutorial/2-train-and-manage-the-model.md)
* [3 - Compare, Register and Deploy the Model](end-to-end-tutorial/3-compare-register-and-deploy-the-model.md)
* [4 - Build the Web Application](end-to-end-tutorial/4-build-the-web-application.md)
* [5 - Summary](end-to-end-tutorial/5-summary.md)
* [Advanced](end-to-end-tutorial/advanced/README.md)
  * [Labeling the data](end-to-end-tutorial/advanced/labeling-the-data.md)
  * [Notebook as a Job](end-to-end-tutorial/advanced/notebook-as-a-job.md)
  * [Custom build the Seldon server](end-to-end-tutorial/advanced/custom-build-the-seldon-server.md)
  * [PrimeHub SDK/CLI Tools](end-to-end-tutorial/advanced/primehub-sdk-cli-tools.md)

## Notebooks

* [Start Notebook](notebooks/start-notebook/README.md)
  * [Advanced Settings](notebooks/start-notebook/advanced-settings.md)
  * [Notebook Tips](notebooks/start-notebook/notebook-tips.md)
* [SSH Server Feature](notebooks/ssh-server-feature/README.md)
  * [VSCode SSH Notebook Remotely](notebooks/ssh-server-feature/vscode-ssh-notebook-remotely.md)
  * [Generate SSH Key Pair](notebooks/ssh-server-feature/generate-ssh-key-pair.md)
  * [Permission Denied](notebooks/ssh-server-feature/permission-denied.md)
  * [Connection Refused](notebooks/ssh-server-feature/connection-refused.md)
* [PrimeHub Notebook Extension](notebooks/primehub-notebook-extension/README.md)
  * [Submit Notebook as Job](notebooks/primehub-notebook-extension/submit-notebook-as-job.md)

## Jobs

* [Jobs/Recurring Jobs](jobs/jobs-recurring-jobs.md)
* [Job Artifacts](jobs/job-artifacts.md)
* [Tutorial](jobs/tutorial/README.md)
  * [(Part1) MNIST classifier training](jobs/tutorial/part1-mnist-classifier-training.md)
  * [(Part2) MNIST classifier training](jobs/tutorial/part2-mnist-classifier-training.md)
  * [(Advanced) Use Job Submission to Tune Hyperparameters](jobs/tutorial/advanced-use-job-submission-to-tune-hyperparameters.md)
  * [(Advanced) Model Serving by Seldon](jobs/tutorial/advanced-model-serving-by-seldon.md)
  * [Job Artifacts Simple Usecase](jobs/tutorial/job-artifacts-simple-usecase.md)

## Models

* [Models](models/models.md)
* [Model Management Configuration](models/model-management-configuration.md)
* [Manage and Deploy Model](models/manage-and-deploy-model.md)

## Deployments

* [Deployments](deployments/deployments.md)
* [Tutorial](deployments/tutorial/README.md)
  * [Model by Pre-packaged Server](deployments/tutorial/model-by-pre-packaged-server.md)
  * [Model by Pre-packaged Server (PHFS)](deployments/tutorial/model-by-pre-packaged-server-phfs.md)
  * [Model by Image built from Language Wrapper](deployments/tutorial/model-by-image-built-from-language-wrapper.md)
* [Pre-packaged servers](deployments/pre-packaged-servers/README.md)
  * [TensorFlow server](deployments/pre-packaged-servers/tensorflow-server.md)
  * [PyTorch server](deployments/pre-packaged-servers/pytorch-server.md)
  * [SKLearn server](deployments/pre-packaged-servers/sklearn-server.md)
  * [Customize Pre-packaged Server](deployments/pre-packaged-servers/customize-pre-packaged-server.md)
  * [Run Pre-packaged Server Locally](deployments/pre-packaged-servers/run-pre-packaged-server-locally.md)
* [Package from Language Wrapper](deployments/package-from-language-wrapper/README.md)
  * [Model Image for Python](deployments/package-from-language-wrapper/model-image-for-python.md)
  * [Model Image for R](deployments/package-from-language-wrapper/model-image-for-r.md)
  * [Reusable Base Image](deployments/package-from-language-wrapper/reusable-base-image.md)
* [Prediction APIs](deployments/prediction-apis.md)
* [Model URI](deployments/model-uri.md)

***

* [Shared Files](shared-files.md)
* [Datasets](datasets.md)

## Apps

* [Apps Overview](apps/apps-overview.md)
* [Tutorial](apps/tutorial/README.md)
  * [Create Your Own App](apps/tutorial/create-your-own-app.md)
  * [Create an MLflow server](apps/tutorial/create-an-mlflow-server.md)
  * [Label Dataset by Label Studio](apps/tutorial/label-dataset-by-label-studio.md)

***

* [Built-in Apps](built-in-apps/README.md)
  * [Code Server](built-in-apps/code-server.md)
  * [Label Studio](built-in-apps/label-studio.md)
  * [MATLAB](built-in-apps/matlab.md)
  * [MLflow](built-in-apps/mlflow.md)
  * [Streamlit](built-in-apps/streamlit.md)

## Group Administration

* [Images](group-administration/images.md)
* [Settings](group-administration/settings.md)

## Platform Administration

* [Admin Portal](platform-administration/admin-portal.md)
  * [Create User](platform-administration/admin-portal/create-user.md)
  * [Create Group](platform-administration/admin-portal/create-group.md)
  * [Assign Group Admin](platform-administration/admin-portal/assign-group-admin.md)
  * [Create/Plan Instance Type](platform-administration/admin-portal/create-plan-instance-type.md)
  * [Add InfuseAI Image](platform-administration/admin-portal/add-infuseai-image.md)
  * [Add Image](platform-administration/admin-portal/add-image.md)
  * [Build Image](platform-administration/admin-portal/build-image.md)
  * [Gitsync Secret for GitHub](platform-administration/admin-portal/gitsync-secret-for-github.md)
  * [Pull Secret for GitLab](platform-administration/admin-portal/pull-secret-for-gitlab.md)
* [User Management](platform-administration/user-management.md)
* [Group Management](platform-administration/group-management.md)
* [Instance Type Management](platform-administration/instance-type-management/README.md)
  * [NodeSelector](platform-administration/instance-type-management/nodeselector.md)
  * [Toleration](platform-administration/instance-type-management/toleration.md)
* [Image Management](platform-administration/image-management/README.md)
  * [Custom Image Guideline](platform-administration/image-management/custom-image-guideline.md)
* [Volume Management](platform-administration/volume-management/README.md)
  * [Upload Server](platform-administration/volume-management/upload-server.md)
* [Secret Management](platform-administration/secret-management.md)
* [Notebooks Admin](platform-administration/notebooks-admin.md)
* [Usage Reports](platform-administration/usage-reports.md)
* [App Settings](platform-administration/app-settings.md)
* [System Settings](platform-administration/system-settings.md)

## Reference

* [InfuseAI Images List](reference/infuseai-images-list.md)
* [Environment Variables](reference/environment-variables.md)
* [Chart Configuration](reference/chart-configuration.md)
* [Multiple Jupyter Notebook Kernels](reference/multiple-jupyter-notebook-kernels.md)

## Configuration

* [How to configure PrimeHub](configuration/how-to-configure-primehub.md)
* [Configure PrimeHub Store](configuration/configure-primehub-store.md)
* [Configure SSH Server](configuration/configure-ssh-server.md)
* [Configure Job Submission](configuration/configure-job-submission.md)
* [Configure Model Deployment](configuration/configure-model-deployment.md)
* [Configure Custom Image Build](configuration/configure-custom-image-build.md)
* [Setup Self-Signed Certificate for PrimeHub](configuration/setup-self-signed-certificate-for-primehub.md)
