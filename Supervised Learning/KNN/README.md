# K-Nearest Neighbors (KNN)

<p align="center">
  <img src="https://miro.medium.com/0*ItVKiyx2F3ZU8zV5" width="600"/>
</p>

---

## Overview

**K-Nearest Neighbors (KNN)** is a supervised machine learning algorithm used for **classification** and **regression**. It predicts outcomes based on the **similarity (distance)** between data points.

KNN is a **non-parametric, instance-based (lazy learning)** algorithm that does not build an explicit model during training. Instead, it stores the dataset and performs computation at prediction time.

This project demonstrates KNN classification, where a data point is assigned a label based on the majority class among its nearest neighbors.

---

## Objective

- Classify data points based on similarity  
- Use distance-based learning  
- Identify patterns in feature space  
- Enable accurate multi-class classification  

---

## What is KNN?

KNN classifies a data point based on its **nearest neighbors in feature space**.

In simple terms:  
A data point is assigned the class that is most common among its closest neighbors.

---

## How It Works

1. Choose the number of neighbors \( k \)  
2. Compute distance between the new point and all training points  
3. Select the **k closest neighbors**  
4. Apply:
   - **Classification** → Majority vote  
   - **Regression** → Average of neighbors  
5. Assign final prediction  

---

## Distance Metrics

### Euclidean Distance

\[
d(x, y) = \sqrt{\sum_{i=1}^{n} (x_i - y_i)^2}
\]

### Manhattan Distance

\[
d(x, y) = \sum_{i=1}^{n} |x_i - y_i|
\]

### Minkowski Distance

\[
d(x, y) = \left( \sum_{i=1}^{n} |x_i - y_i|^p \right)^{1/p}
\]

---

## Prediction Formulas

### Classification (Majority Voting)

\[
\hat{y} = \text{mode}(y_1, y_2, ..., y_k)
\]

### Regression (Averaging)

\[
\hat{y} = \frac{1}{k} \sum_{i=1}^{k} y_i
\]

### Weighted KNN (Optional)

\[
\hat{y} = \frac{\sum_{i=1}^{k} w_i y_i}{\sum_{i=1}^{k} w_i}, \quad \text{where } w_i = \frac{1}{d(x, x_i)}
\]

---

## Methodology

- **Classification by Proximity** → Majority voting among nearest neighbors  
- **Regression via Averaging** → Mean of neighbor values  
- **Lazy Learning** → No training phase  
- **Local Approximation** → Decisions based on nearby points  
- **Pattern Recognition** → Similar points cluster together  

---

## Key Concepts

- **K Value** → Number of neighbors considered  
- **Distance Metric** → Defines similarity  
- **Feature Scaling** → Ensures fair distance calculation  
- **Local Decision Making** → Focus on neighborhood patterns  

---

## Choosing the Right K

- Small \( k \) → High variance, sensitive to noise  
- Large \( k \) → Low variance, may underfit  

Optimal \( k \) is typically selected using cross-validation.

---

## Key Idea

**Similar data points exist close to each other in feature space.**

---

## Advantages

- Simple and intuitive  
- No training phase required  
- Works well with small datasets  
- Supports multi-class classification  

---

## Limitations

- Computationally expensive at prediction time  
- Sensitive to feature scaling  
- Performance depends on \( k \)  
- Affected by noise and outliers  

---

## Applications

- Recommendation systems  
- Image classification  
- Pattern recognition  
- Medical diagnosis  
- Fraud detection  

---

## Conclusion

KNN is a simple yet powerful algorithm based on **distance-driven similarity**. Its effectiveness depends heavily on **feature scaling**, **distance metric**, and **choice of \( k \)**.

---
