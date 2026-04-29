# Linear Regression

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/3/3a/Linear_regression.svg" width="600"/>
</p>

---

## Overview

**Linear Regression** is a supervised machine learning algorithm used to model the **linear relationship** between input features and a continuous target variable.

It estimates a best-fit line that minimizes the difference between actual and predicted values. :contentReference[oaicite:0]{index=0}

---

## Objective

- Model relationships between variables  
- Predict continuous outcomes  
- Minimize prediction error  
- Understand feature impact on target variable  

---

## What is Linear Regression?

Linear Regression predicts a target variable using a linear equation.

In simple terms:  
It finds the best straight line that fits the data.

---

## Model Representation

### Simple Linear Regression

ŷ = β₀ + β₁x  

Where:  
- β₀ → Intercept  
- β₁ → Slope  
- x → Input feature  

### Multiple Linear Regression

ŷ = β₀ + β₁x₁ + β₂x₂ + ... + βₙxₙ  

This extends the model to multiple features. :contentReference[oaicite:1]{index=1}

---

## Loss Function

### Mean Squared Error (MSE)

MSE = (1/n) Σ (yᵢ − ŷᵢ)²  

The goal is to minimize this error to find the best-fit line.

---

## Least Squares Solution

Linear Regression finds parameters by minimizing squared error.

### Line Equation

y = mx + c  

### Slope (m)

m = [nΣxy − (Σx)(Σy)] / [nΣx² − (Σx)²]

### Intercept (c)

c = (Σy − mΣx) / n  

These formulas compute the **best-fit line** using least squares. :contentReference[oaicite:2]{index=2}

---

## Optimization (Gradient Descent)

Parameters can also be learned iteratively:

w = w − α · ∇J(w)  
b = b − α · ∂J/∂b  

Where:  
- α → Learning rate  
- J(w) → Cost function  

---

## Normal Equation (Closed Form)

An alternative to gradient descent:

θ = (XᵀX)⁻¹ Xᵀy  

This directly computes optimal parameters without iteration.

---

## Types of Linear Regression

- **Simple Linear Regression** → One feature  
- **Multiple Linear Regression** → Multiple features  
- **Polynomial Regression** → Non-linear relationships via transformations  

---

## Methodology

- Fit a linear equation to data  
- Minimize error using least squares or gradient descent  
- Evaluate using regression metrics  
- Interpret coefficients  

---

## Key Concepts

- Linearity assumption  
- Residuals (errors)  
- Overfitting vs underfitting  
- Feature scaling (important for optimization)  

---

## Advantages

- Simple and interpretable  
- Computationally efficient  
- Works well with linear relationships  
- Strong baseline model  

---

## Limitations

- Assumes linear relationship  
- Sensitive to outliers  
- Multicollinearity issues  
- Cannot capture complex patterns  

---

## Applications

- House price prediction  
- Sales forecasting  
- Risk analysis  
- Financial modeling  
- Demand prediction  

---

## References

- https://www.geeksforgeeks.org/machine-learning/ml-linear-regression/  
- https://www.geeksforgeeks.org/maths/least-square-method/  
- https://scikit-learn.org/stable/modules/linear_model.html  
- https://developers.google.com/machine-learning/crash-course/linear-regression  
- https://link.springer.com/book/10.1007/978-0-387-84858-7  

---
