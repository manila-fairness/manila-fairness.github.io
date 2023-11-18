# Step-by-Step Tutorial

In this tutorial you will use MANILA to perform a _fairness_ and _effectiveness_ evaluation of different machine learning settings (i.e., machile learning model and fairness-enhancing methods) to predict recidivism of condemned people using the well-known [COMPAS](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing) dataset.

In particular you will evaluate the fairness and effectiveness of the following settings using the following metrics:

- **Settings:** _Logistic Regression (LR)_, and _Random Forest (RF)_ with and without the following fairness-enhancing methods: _Reweighing_, and _Debiaser for Multiple Variables_ (DEMV).
- **Metrics:** _Accuracy_, _Disparate Impact_, _Equalized Odds_.

Finally, you will use the _Harmonic Mean_ as aggregation function to obtain a single score for each setting.

MANILA will independently evaluate each setting using the selected metrics and identify the best setting according to the selected aggregation function.

In the following, we show the steps to perform the evaluation.

## 1. Obtain the dataset

First, you need to obtain the dataset. In this tutorial, we will use the COMPAS dataset. The dataset can be downloaded from [here](./_static/compas.csv).

At this time, MANILA supports only tabular datasets in different formats (e.g., CSV, Excel, JSON, etc.). The format of the dataset can be specified from the interface of MANILA.

## 2. Access MANILA

Access MANILA from the <a href="https://sobigdata.d4science.org/group/sobigdata.it/manila-univaq" target="_blank">SoBigData RI</a>. If not already done, you need to register to the system, the registration is free.

After registering to the system you will find MANILA in the catalogue of services by clicking on the catalogue icon in the top bar and by going on the _SoBigData Services and Products_ organisation.

The interface of MANILA is shown below:
![manila](./_static/manila.png)

## 3. Using MANILA

MANILA is divided into different sections that allow you to specify the different features of your experiment.

### 3.1. Dataset
