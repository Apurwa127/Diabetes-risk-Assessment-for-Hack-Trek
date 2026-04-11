# AI-Powered Diabetes Risk Assessment Tool

## Overview
This project is a machine learning-based system that predicts diabetes risk using patient health data. It provides a prediction, probability score, and an automated risk summary to support early screening.

---

## Problem
Diabetes often goes undetected until serious complications occur. Early prediction can help individuals take preventive action and seek medical care sooner.

---

## Solution
This project uses a Random Forest model to predict diabetes risk based on features such as glucose level, BMI, age, and other health indicators.

The system:
- Predicts diabetes (Yes/No)
- Provides probability score
- Classifies risk level (Low / Moderate / High)
- Generates an automated summary

---

## Dataset
The dataset includes the following features:
- Pregnancies  
- Glucose  
- Blood Pressure  
- Skin Thickness  
- Insulin  
- BMI  
- Diabetes Pedigree Function  
- Age  

---

## Data Preprocessing
- Removed duplicate values  
- Replaced zero values with missing values in medical features  
- Filled missing values using median  
- Scaled features using StandardScaler  

---

## Model Selection
The following models were tested:
- Logistic Regression  
- Decision Tree  
- Random Forest  

Random Forest was selected as the best model using GridSearchCV with Stratified K-Fold cross-validation.

---

## Results
- Test Accuracy: ~99.6%  
- ROC-AUC: ~0.99  
- Cross-validation Accuracy: ~99.3%  

---

## Automation Feature
The system automatically generates a risk summary based on the prediction, helping users quickly understand the results.

---

## Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Google Colab  

---

## How to Run
1. Install required libraries:
2. Open the notebook:

3. Run all cells and test predictions

---

## Limitations
- The dataset may not reflect real-world variability  
- This model is not intended for clinical diagnosis  

---

## Future Work
- Add explainability (SHAP)  
- Deploy as a web app  
- Use larger datasets  

---

## Disclaimer
This project is for educational purposes only and should not be used for medical diagnosis.
