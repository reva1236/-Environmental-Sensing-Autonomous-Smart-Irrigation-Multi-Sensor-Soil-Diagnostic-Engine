# Environmental Sensing Autonomous Smart Irrigation Multi Sensor Soil Diagnostic Engine

## Project Overview
Using tabular datasets compiled from localized environmental telemetry (ambient temperature, relative humidity, atmospheric pressure, solar radiation, NPK indices), build an ensemble model (XGBoost) to predict real-time soil moisture depletion rates and generate automated irrigation control variables.
---
## Features

* Supervised and Unsupervised Learning
* Linear Regression
* Logistic Regression
* Random Forests
* Gradient Boosting Machines (GBM)
* AdaBoost
* XGBoost
* Regularization (L1 & L2)
* Bias–Variance Trade-off
* Cross Validation
* Model Evaluation (ROC-AUC, Precision, Recall, F1-Score)
* Feature Importance Analysis
* Data Leakage Prevention
---

## Technologies Used

* Python
* Scikit-Learn
* XGBoost
* LightGBM
* Joblib

---

## Core Theoretical Concepts

### Supervised vs. Unsupervised Learning

* **Supervised Learning**

  * Labelled data
  * Classification
  * Regression

* **Unsupervised Learning**

  * Unlabelled data
  * Clustering
  * Association
  * Dimensional Reduction

---


### Tree-Based Ensembles

* Random Forests
* Gradient Boosting Machines (GBM): Average + learning rate × Tree 1 + learning rate × Tree 2 + ...
* XGBoost: Similarity Score → Gain → Prune

---

### Regularization

**L1 (Lasso)**
Allows the parameters not necessary to become 0 while in ridge they tend to 0.

**L2 (Ridge)**

* Introduces bias to reduce variance.
* Can be used when the number of parameters are less.
* Ridge regression penalty must be minimized.

---

### Bias–Variance Trade-off

Bias
The inability of an ML method to capture the true relation is called bias.

Variance
The inability of an ML method to perform for the testing set is called variance.

Methods:
* Regularization
* Boosting
* Bagging
---

### Cross-Validation Mechanics

* Which ML method is the best.
* Estimating parameters – Training the algorithm.
* If the ML model works – Testing the algorithm.
* Cross validation uses different blocks for training and testing.

Types
* Dividing into 4 blocks → Four-fold classification.
* Using 1 record for test and rest for training → Leave-one-out validation.
* 10-fold is most common.

---

## Dataset

The project uses tabular datasets compiled from localized environmental telemetry containing:

* Ambient Temperature
* Relative Humidity
* Atmospheric Pressure
* Solar Radiation
* NPK Indices

---

## Learning Outcomes

* Evaluate models using:
  * Precision
  * Recall
  * ROC-AUC
  * F1-Score
* Perform Feature Importance Analysis
* Avoid Data Leakage across Training Splits

---

## Author
**Reva Kulkarni**
