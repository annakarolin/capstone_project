This repository contains the final project done as part of machine learning course done with LaunchEd.

# Applicant Compensation Prediction

### Project Overview
This project predicts **applicants’ expected compensation** using machine learning regression models.  
Using a dataset of **25,000 applicant profiles**, the study explores how factors such as **education**, **professional experience**, and **current salary (CTC)** influence expected salary.  

The goal was to identify the most accurate and reliable models for forecasting compensation expectations in a professional recruitment context.

---

### Objective
To benchmark multiple regression models and determine the best-performing algorithms for predicting expected compensation, while uncovering key drivers behind salary expectations.

---

### Models Compared
- Linear Regression  
- Support Vector Regression (SVR)  
- Random Forest Regressor  
- Gradient Boosting Regressor  
- XGBoost Regressor  
- AdaBoost Regressor  
- Multi-Layer Perceptron (MLP)

---

### Data Preparation
To ensure data consistency and quality:
- Missing values were imputed using **mean** (numerical) and **mode** (categorical).  
- **Categorical variables** were encoded using one-hot encoding.  
- **Feature scaling** was applied to all numerical features.  
- **Outliers** were identified and capped using boxplot and z-score analysis.  
- The dataset was split into **70% training** and **30% testing** sets.  

---

### Results Summary
| Model | R² (Test) | RMSE (Test) | Notes |
|:------|:----------:|:------------:|:------|
| Linear Regression | 0.906 | 0.205 | Performs well but limited by linearity |
| Random Forest (tuned) | **0.929** | **0.178** | Excellent accuracy & generalization |
| Gradient Boosting (tuned) | **0.928** | **0.180** | Robust and stable performance |
| XGBoost (tuned) | **0.928** | **0.180** | Fast, scalable, and highly accurate |
| MLP (tuned) | 0.916 | 0.195 | Improved after tuning, slight variance |

 **Best Models:** Random Forest, XGBoost, and Gradient Boosting  
 **Performance:** R² ≈ 0.93 | RMSE ≈ 0.18  

---

### Key Insights
- **Current CTC**, **total experience**, and **education level** are the strongest predictors of expected salary.  
- **Ensemble models** (Random Forest, Gradient Boosting, XGBoost) outperform linear and neural models.  
- Tuned ensemble methods achieve an excellent balance between **bias and variance**, ensuring robust predictions.  

---
