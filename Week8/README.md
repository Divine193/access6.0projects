# 📋 Final Capstone Project

## 📕 Dataset Used - <a href="https://www.kaggle.com/datasets/mosapabdelghany/medical-insurance-cost-dataset" target="_blank"> Medical Insurance Cost </a>

## 🎯 Problem Statements
- There were two main objectives of this project:
  - **Regression task** : Predict the cost of medical charges
  -  **Classification task** : create a new column that differentiates high paying and low paying customers then build a classification model to predict it.
 
## Models Built
### Regression Models :
- Linear Regression
- DecisionTree Regressor
- Random Forest
- XGBoost

### Classification Models :
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

## 📊 Key findings
- **Primary Drivers of Cost:** Smoking status is the most significant predictor of insurance charges. Age and BMI follow as secondary but critical factors.

- **Predictive Success:** Regression models were able to estimate insurance charges with high accuracy with Random Forest Regressor being the one that captured most of the instances, while classification models (specifically a tuned Random Forest) successfully categorized risk levels or statuses using combined numerical and one-hot encoded categorical features.

- **Demographic Tiers:** The data suggests distinct "charge tiers," where individuals with similar ages and BMIs see drastically different costs depending on whether they smoke.

- **Residual Analysis:** The plot of the residuals against the predicted charges shows a cone shape; This means that the variance of the errors are not constant; The model's variance increases as charges go up.This is common in insurance where high cost outliers behave differently than the average patients.


  
