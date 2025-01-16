Step-by-Step Tutorial
======================

In this tutorial you will use MANILA to perform a *fairness* and *effectiveness* evaluation of different machine learning settings (i.e., machile learning model and fairness-enhancing methods) to predict recidivism of condemned people using the `COMPAS <https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing>`_ dataset.

In particular, you will evaluate the fairness and effectiveness of the following settings using the following metrics:

- **Settings:** *Logistic Regression*, and *Random Forest* with and without the following fairness-enhancing methods: *Reweighing*, and *Debiaser for Multiple Variables (DEMV)*.
- **Metrics:** *Accuracy*, *Disparate Impact*, *Equalized Odds*.

Finally, you will use the *Harmonic Mean* as aggregation function to obtain a single score for each setting.

MANILA will independently evaluate each setting using the selected metrics and identify the best setting according to the selected aggregation function.

In the following, we show the steps to perform the evaluation.

.. toctree::
  dataset
  access
  use
  results
  :maxdepth: 2
