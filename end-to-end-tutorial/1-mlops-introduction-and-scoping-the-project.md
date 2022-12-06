# 1 - MLOps Introduction and Scoping the Project

### What is MLOps?

Machine Learning Operations, also called MLOps, is a process of training and deploying models into the production environment. Before we use the MLOps method to generate the model production service, we need to define several steps to prove that we can let our machine learning model into production.

### MLOps Pipeline Introduction

In the MLOps pipeline, We implement the following stages:

<figure><img src="../.gitbook/assets/primehub-end-to-end-tutorial-mlops_pipeline_introduction.png" alt=""><figcaption><p>MLops pipeline</p></figcaption></figure>

#### 1. Scoping

Plan and check that the project or product scope is suitable for Machine Learning Model. You can use the following form to evaluate your project.

The example table of project scope:

<figure><img src="../.gitbook/assets/primehub-end-to-end-tutorial-project-scope-example.png" alt=""><figcaption><p>project scope table</p></figcaption></figure>

#### 2. Data Engineering

Build the data processing pipeline, we can call it the DataOps pipeline. including the following method:

* **E:** Data **E**xtraction - Collect the data
* **T**: **T**ransform the data to be the dataset and label the dataset.
* **L**: **L**oad the dataset into a database or file system.
* **P**: Check the data **P**rofiling content. We can use the dashboard to show the data insight and keep modifying the Data ETL pipeline.
* **A:** Check the data quality and **A**ssertion status. We must ensure that the dataset quality can be assured before using it.

{% hint style="info" %}
InfuseAI provides the open-source data assertion and profiling tool - _**Piperider**_ to check the data quality toolkit for data professionals. Visit [here](https://www.piperider.io/) for the detail.
{% endhint %}

#### 3. Model Engineering

Here are some steps to build up a modeling pipeline.

1. **Model Building**: Initial the model pipeline and callback method.
2. **Model Training**: Train the data by the machine learning or deep learning Model. At the same time, we need to define the measurement and track the model performance. For example, confusion matrix methods or accuracy metrics.
3. **Model Evaluation**: Check the model is ready for deployment. For example, if the accuracy rate is bigger than 0.95, then we can change to the new model.
4. **Model Registry:** Register the model and put the model into the production waiting line.
5. **Model** **Deployment**: Use the _Dockerize_ method to package the model and deploy it into the cloud or edge devices as endpoints. The package method could be an API server or serverless method.
6. **Model Monitoring**: Monitor the model service performance, which contains two parts:
   1. Monitor the infrastructure where we deploy: E.g. load, usage, storage, and health.
   2. Monitor the model for its performance: Model and data performance that we need to retrain or not.

### The scope of the showcase: Screw defect detection

In this demo showcase, we can use the project table to define the project scope and check the information:

| Variable              | Content                                                                                                            |
| --------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Project Name          | Screw defect detection                                                                                             |
| Dataset               | Screw dataset                                                                                                      |
| Dataset Resource Link | [https://www.kaggle.com/datasets/ruruamour/screw-dataset](https://www.kaggle.com/datasets/ruruamour/screw-dataset) |
| Model                 | Image Classification Model                                                                                         |
| Code language         | Python 3.7 + Tensorflow 2.5                                                                                        |
| Project Goal          | Use the computer vision recognition method to analyze the screw images.                                            |
| Measurement           | Accuracy, Loss                                                                                                     |
| Delivery              | <p>1. Metrics information<br>2. deployment service<br>3. Application service UI</p>                                |

### Next Section

In the next part, we will use the PrimeHub Platform to label the model.
