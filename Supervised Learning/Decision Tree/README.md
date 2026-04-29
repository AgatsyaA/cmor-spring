# Decision Tree

<p align="center">
  <img src="https://www.cfoselections.com/hubfs/when%20to%20use%20a%20decision%20tree%20for%20business%20planning.png" width="600"/>
</p>

---

## Overview

A **Decision Tree** is a supervised machine learning algorithm used for **classification** and **regression**. It models decisions using a **tree-like structure**, where data is recursively split based on feature conditions to generate predictions.

It is a **non-parametric model** that is highly interpretable and widely used as a foundation for ensemble methods such as Random Forests and Gradient Boosting.

---

## Objective

- Learn decision rules from data  
- Partition feature space into meaningful regions  
- Enable accurate classification and regression  
- Provide interpretable model outputs  

---

## What is a Decision Tree?

A Decision Tree splits data into subsets based on feature values, forming a structure of nodes and branches.

In simple terms:  
The model asks a sequence of questions to arrive at a final prediction.

---

## How It Works

1. Select the best feature to split the data  
2. Apply a splitting criterion (e.g., entropy, Gini)  
3. Partition the dataset into subsets  
4. Repeat recursively for each subset  
5. Stop when a stopping condition is met (e.g., max depth, pure node)  

---

## Structure

- **Root Node** → Represents the entire dataset  
- **Decision Nodes** → Apply feature-based conditions  
- **Branches** → Represent outcomes of splits  
- **Leaf Nodes** → Contain final predictions  

---

## Key Concepts

- **Entropy** → Measures randomness in data  
- **Information Gain** → Reduction in entropy after a split  
- **Gini Impurity** → Measures probability of misclassification  
- **Overfitting** → Model learns noise instead of pattern  

---

## Splitting Criteria (Formulas)

### Entropy  
Entropy(S) = − Σ pᵢ log₂(pᵢ)

### Information Gain  
IG(S, A) = Entropy(S) − Σ (|Sᵥ| / |S|) · Entropy(Sᵥ)

### Gini Impurity  
Gini(S) = 1 − Σ (pᵢ)²  

---

## Types of Decision Trees

- **Classification Trees** → Predict categorical labels  
- **Regression Trees** → Predict continuous values  

---

## Methodology

- Recursive partitioning of feature space  
- Greedy selection of best split at each step  
- Tree growth followed by pruning for optimization  
- Local decision-making at each node  

---

## Advantages

- Easy to understand and interpret  
- Requires minimal data preprocessing  
- Handles both numerical and categorical data  
- Captures non-linear relationships  

---

## Limitations

- Prone to overfitting  
- Sensitive to small variations in data  
- Can create overly complex trees  
- Greedy splitting may not yield global optimum  

---

## Common Techniques

- **Pruning** → Reduces overfitting by trimming branches  
- **Max Depth Control** → Limits tree size  
- **Minimum Samples Split** → Avoids weak splits  
- **Feature Selection** → Improves split quality  

---

## Applications

- Customer segmentation  
- Credit risk analysis  
- Medical diagnosis  
- Fraud detection  

---

## References

- https://www.geeksforgeeks.org/decision-tree/  
- https://scikit-learn.org/stable/modules/tree.html  
- https://www.ibm.com/topics/decision-trees  

---
