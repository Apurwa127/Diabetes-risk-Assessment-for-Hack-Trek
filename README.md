# AI-Powered Diabetes Risk Assessment Tool

---

## Overview
This project is a machine learning-based system that predicts diabetes risk using patient health data. It provides a prediction, probability score, and an automated risk summary to support early screening.

---

## Problem
Diabetes often goes undetected until serious complications occur. Early prediction can help individuals take preventive action and seek medical care sooner.

---

## Solution
This project uses machine learning models to predict diabetes risk based on features such as glucose level, BMI, age, and other health indicators.

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
- Performed train-test split  
- Scaled features using StandardScaler (fit on training data only to avoid data leakage)  

---

## Model Selection
The following models were tested:

- Logistic Regression (baseline model)  
- Decision Tree  
- Random Forest (final model)  

The Random Forest model was selected as the final model due to its superior performance and ability to capture complex relationships in the data.

To ensure the results were reliable and not model-specific, Logistic Regression was used as a baseline for comparison. While it provided balanced and interpretable results, its predictive performance was lower than Random Forest.

Hyperparameter tuning for Random Forest was performed using GridSearchCV with Stratified K-Fold cross-validation.

---

## Results

### Logistic Regression (Baseline)
- Accuracy: ~75%  
- ROC-AUC: ~0.83  

### Random Forest (Final Model)
- Test Accuracy: ~99.6%  
- ROC-AUC: ~0.99  
- Cross-validation Accuracy: ~99.3%  

---

## Model Validation
- Ensured no data leakage by applying preprocessing only on training data  
- Used a separate test set for evaluation  
- Applied cross-validation to assess model stability  

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
1. Install required libraries  
2. Open the notebook  
3. Run all cells and test predictions  

---

## Limitations
- The dataset may not reflect real-world variability  
- Model performance may be optimistic due to dataset simplicity  
- This model is not intended for clinical diagnosis  

---

## Future Work
- Add explainability (SHAP)  
- Deploy as a web app  
- Use larger datasets  

---

## Disclaimer
This project is for educational purposes only and should not be used for medical diagnosis.
