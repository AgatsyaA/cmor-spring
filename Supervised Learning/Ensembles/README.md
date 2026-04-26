# Ensemble Learning: Regression and Classification

<div align="center">
  <img src="https://www.ibm.com/adobe/dynamicmedia/deliver/dm-aid--fc4f06fb-b27c-424b-9180-3163e7d2825e/ensemble-learning-boosting.png" width="700"/>
</div>

---

## Overview

This project demonstrates practical implementations of ensemble learning techniques for both regression and classification problems.

Ensemble learning improves accuracy, robustness, and generalization by combining multiple models.

---

## Key Concepts

- Bagging (Bootstrap Aggregation): Reduces variance  
- Boosting: Reduces bias by sequential learning  
- Stacking: Combines multiple models using a meta-learner  

---

## Project Files

- `CODE Regressor.ipynb` — Ensemble methods for regression  
- `CODE Classification.ipynb` — Ensemble methods for classification  

---

## Regression (CODE Regressor.ipynb)

### Implementations
- Data preprocessing  
- Base models (Linear Regression, Decision Trees)  
- Ensemble models:
  - Random Forest Regressor  
  - Gradient Boosting Regressor  

### Evaluation Metrics
- Root Mean Squared Error (RMSE)  
- R-squared (R² Score)  

---

## Classification (CODE Classification.ipynb)

### Implementations
- Data preprocessing  
- Base classifiers (Logistic Regression, Decision Tree)  
- Ensemble models:
  - Random Forest Classifier  
  - AdaBoost / Gradient Boosting  
  - Voting Classifier  

### Evaluation Metrics
- Accuracy  
- Precision and Recall  
- Confusion Matrix  

---

## Workflow

1. Load dataset  
2. Preprocess data  
3. Train baseline models  
4. Apply ensemble techniques  
5. Evaluate performance  

---

## Why Ensemble Learning

| Problem            | Solution                |
|-------------------|------------------------|
| High variance      | Bagging                |
| High bias          | Boosting               |
| Model limitations  | Stacking               |

---

## Technology Stack

- Python  
- Scikit-learn  
- Pandas, NumPy  
- Matplotlib  

---

## How to Run

```bash
pip install numpy pandas scikit-learn matplotlib
jupyter notebook
