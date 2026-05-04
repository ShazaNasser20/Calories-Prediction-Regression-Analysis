#  Calories Prediction & Regression Analysis

##  Project Overview

This project analyzes a fitness dataset to understand the factors affecting calories burned and builds multiple regression models to predict calorie expenditure.

The workflow combines **Exploratory Data Analysis (EDA)** with **Machine Learning modeling** to compare different regression techniques.

---

##  Dataset Information

The dataset includes:

* Age
* Height
* Weight
* Duration
* Heart Rate
* Body Temperature
* Gender
* Calories (Target Variable)

---

##  Data Preprocessing

* Removed outliers using **IQR method**
* Encoded categorical variable:

  * Gender → One-Hot Encoding
* Feature scaling applied using:

  * **StandardScaler**
* Dropped unnecessary column:

  * User_ID

---

##  Exploratory Data Analysis

The following analyses were performed:

* Distribution plots for all numerical features
* Boxplots for outlier detection
* Scatter plots to analyze relationships:

  * Duration vs Calories
  * Heart Rate vs Calories
* Correlation heatmap

---

##  Key Observations

* Calories strongly increase with **Duration**
* **Heart Rate** is highly correlated with calories burned
* Weight and Body Temperature also contribute
* Data cleaning improved distribution stability

---

##  Machine Learning Models

The following models were trained and compared:

* Linear Regression (Normal Equation)
* Linear Regression (Gradient Descent using SGDRegressor)
* Ridge Regression
* Lasso Regression
* Elastic Net

---

##  Model Evaluation

* Evaluation metric used: **R² Score**

###  Comparison:

* Linear Regression performed as a strong baseline
* Ridge improved stability with regularization
* Lasso performed feature selection (zero coefficients)
* ElasticNet balanced between Ridge and Lasso
* Gradient Descent showed comparable performance

---

##  Visualization

* Actual vs Predicted plots for each model
* Feature importance visualization
* Lasso coefficient shrinkage

---

##  Final Insights

* **Duration** is the most influential feature
* **Heart Rate** plays a major role in calorie prediction
* Regularization improves model generalization
* Lasso helps in feature selection

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

##  Future Work

* Try advanced models (Random Forest, XGBoost)
* Hyperparameter tuning
* Cross-validation
* Deploy as a web app

```
