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

**Bias**
The inability of an ML method to capture the true relation is called bias.

**Variance**
The inability of an ML method to perform for the testing set is called variance.

**Methods:**
* Regularization
* Boosting
* Bagging
---

### Cross-Validation Mechanics

* Which ML method is the best.
* Estimating parameters – Training the algorithm.
* If the ML model works – Testing the algorithm.
* Cross validation uses different blocks for training and testing.

**Types**
* Dividing into 4 blocks → Four-fold classification.
* Using 1 record for test and rest for training → Leave-one-out validation.
* 10-fold is most common.

---

## Dataset
The dataset is taken from https://www.kaggle.com/datasets/datasetengineer/smart-farming-data-2024-sf24

Dataset contains:
The dataset contains 4800 records with 28 features (23 original features and 5 derived features), each representing critical environmental and soil parameters, along with specific crop-related metrics. These features include:
* N (ppm): Nitrogen content in the soil.
* P (ppm): Phosphorus content in the soil.
* K (ppm): Potassium content in the soil.
* Temperature (°C): Ambient temperature recorded at the farm.
* Humidity (%): Relative humidity at the location.
* pH: Soil pH level, indicating acidity or alkalinity.
* Rainfall (mm): Amount of rainfall received.
* Label: Type of crop associated with the recorded conditions (e.g., rice).
* Soil Moisture (%): Percentage of water content in the soil.
* Soil Type: Type of soil (1 = Sandy, 2 = Loamy, 3 = Clay).
* Sunlight Exposure (hrs/day): Average daily sunlight exposure.
* Wind Speed (km/h): Wind speed at the farm.
* CO2 Concentration (ppm): Carbon dioxide concentration in the air.
* Organic Matter (%): Percentage of organic material in the soil.
* Irrigation Frequency (times/week): Frequency of irrigation.
* Crop Density (plants/m²): Number of plants per square meter.
* Pest Pressure (index): Level of pest infestation.
* Fertilizer Usage (kg/ha): Amount of fertilizer applied per hectare.
* Growth Stage: Current growth stage of the crop (1 = Seedling, 2 = Vegetative, 3 = Flowering).
* Urban Area Proximity (km): Distance to the nearest urban area.
* Water Source Type: Type of water source used for irrigation (1 = River, 2 = Groundwater, 3 = Recycled).
* Frost Risk (index): Risk of frost occurrence.
* Water Usage Efficiency (L/kg): Efficiency of water usage per kilogram of crop yield.

Derived Features:
In addition to the original attributes, the dataset includes 5 derived features that provide deeper insights into the interactions between environmental conditions and crop performance:

* Temperature-Humidity Index (THI): A composite measure that evaluates potential crop stress due to specific heat and moisture conditions.
* Nutrient Balance Ratio (NBR): Reflects the balance between nitrogen, phosphorus, and potassium in the soil.
* Water Availability Index (WAI): Combines soil moisture and rainfall to assess overall water availability for crops.
* Photosynthesis Potential (PP): Estimates the potential for photosynthesis based on sunlight exposure, CO2 concentration, and temperature.
* Soil Fertility Index (SFI): A composite metric that assesses soil fertility based on organic matter content and NPK levels.

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
