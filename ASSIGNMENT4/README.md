# Ensemble Prediction and Decision Tree Model Evaluation

## Overview
This project implements and evaluates multiple machine learning classifiers on the Breast Cancer Wisconsin (Diagnostic) Dataset. The goal is to compare single models (Decision Tree) with ensemble methods (AdaBoost, Gradient Boosting, XGBoost, Random Forest, and Stacked Models) using 5-Fold Cross-Validation and hyperparameter tuning.

## Features
- Data preprocessing (handling missing values, encoding, standardization)  
- Exploratory Data Analysis (class balance and feature correlation heatmap)  
- Model training with:  
  - Decision Tree  
  - AdaBoost  
  - Gradient Boosting  
  - XGBoost  
  - Random Forest  
  - Stacked Ensemble (SVM, Naïve Bayes, Decision Tree)  
- Hyperparameter tuning with RandomizedSearchCV  
- Model evaluation using:  
  - Accuracy and F1 Score  
  - Cross-validation results  
  - Confusion matrix  
  - ROC curves and AUC  
  - Classification reports  

## Dataset
- **Source**: Breast Cancer Wisconsin (Diagnostic) dataset (`wdbc.data`)  
- **Samples**: 569  
- **Features**: 30 numerical attributes  
- **Target**: Diagnosis (Malignant = 1, Benign = 0)  

## Libraries Used
- **pandas**: data handling  
- **numpy**: numerical operations  
- **matplotlib, seaborn**: visualization  
- **scikit-learn**: preprocessing, model building, tuning, evaluation  
- **xgboost**: XGBoost implementation  

## Results
- **Best Model**: AdaBoost with an average validation accuracy of **97.7%**  
- **Decision Tree** alone underperformed compared to ensemble methods  
- **Random Forest** and **Stacking** also achieved strong performance (~96%)  
- **No severe overfitting** observed across models  

## Key Observations
1. AdaBoost achieved the highest validation accuracy.  
2. Decision Tree showed weaker performance compared to ensemble methods.  
3. Random Forest tuning (max depth, n_estimators) provided minimal improvements.  
4. Stacking improved over weaker base models but did not surpass AdaBoost.  

## Learning Outcomes
- Implementation of multiple ML algorithms and ensembles  
- Understanding hyperparameter tuning and cross-validation  
- Comparison of model performance with appropriate metrics  
- Insights into model generalization, underfitting, and overfitting  
- Ability to report and present machine learning experiments effectively  
