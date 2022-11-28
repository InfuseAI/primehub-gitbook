# MLflow

Enterprise Applicable to Enterprise EditionCommunity Applicable to Community Edition

### Introduction

MLflow is an open source platform to manage the ML lifecycle, including experimentation, reproducibility, deployment, and a central model registry.

| Property         | Description                                                   |
| ---------------- | ------------------------------------------------------------- |
| App Image        | [`larribas/mlflow`](https://hub.docker.com/r/larribas/mlflow) |
| Official Website | https://mlflow.org/                                           |

### Screenshots

### Usage

1. Create a MLflow app
2. There are two predefined environment variables
3. The default value of backend store uri `sqlite:///$(PRIMEHUB_APP_ROOT)/mlflow.db` is the sqlite db under the group volume
4. The default value of artifact root `$(PRIMEHUB_APP_ROOT)/mlruns` is the folder under the group volume
5. You can change these environment variables to use your own settings if you want
6. After created, MLflow is ready to manage your ML lifecycle
