# Principal Component Analysis (PCA)

<p align="center">
  <img src="https://devopedia.org/images/article/139/4543.1548137789.jpg" width="600"/>
</p>

---

## Overview

**Principal Component Analysis (PCA)** is a dimensionality reduction technique used to transform high-dimensional data into a lower-dimensional space while preserving as much **variance** as possible.

It achieves this by projecting data onto a new set of **orthogonal axes (principal components)** that capture maximum variance in descending order.

PCA is widely used for **data compression, visualization, noise reduction**, and as a preprocessing step for machine learning models.

---

## Learning Objectives

- Understand dimensionality reduction  
- Learn how PCA transforms data into principal components  
- Analyze variance explained by each component  
- Apply PCA for visualization and preprocessing  

---

## Problem Formulation

Given a dataset:

X ∈ ℝⁿˣᵈ

PCA finds a transformation:

X → Z

Where:
- Z is a lower-dimensional representation  
- Variance retained in Z is maximized  

---

## Key Concepts

### Variance
Measures spread in data. PCA maximizes variance along new axes.

### Principal Components
New orthogonal directions formed as linear combinations of original features.

### Orthogonality
Principal components are uncorrelated.

### Explained Variance
Quantifies how much information each component retains.

---

## Mathematical Intuition

1. Standardize the dataset  
2. Compute covariance matrix  
3. Perform eigen decomposition  
4. Sort components by eigenvalues  
5. Select top K components  
6. Project data onto new space  

---

## Algorithm Workflow

1. Normalize or standardize data  
2. Compute covariance matrix  
3. Calculate eigenvalues and eigenvectors  
4. Sort components by variance explained  
5. Select top K components  
6. Transform data  

---

## Formulas

### Mean Centering

X_centered = X − μ  

---

### Covariance Matrix

Σ = (1/n) XᵀX  

---

### Eigenvalue Decomposition

Σv = λv  

Where:  
- v → Eigenvector (principal component)  
- λ → Eigenvalue (variance explained)  

---

### Projection (Dimensionality Reduction)

Z = XW  

Where:  
- W → Matrix of top K eigenvectors  
- Z → Transformed data  

---

### Explained Variance Ratio

Explained Variance = λᵢ / Σ λⱼ  

---

## Choosing Number of Components

### Explained Variance Threshold
Select components capturing ~90–95% variance.

---

### Scree Plot
Plot eigenvalues vs component index to identify diminishing returns.

---

## Advantages

- Reduces dimensionality effectively  
- Improves computational efficiency  
- Removes redundancy and noise  
- Enables visualization (2D/3D)  

---

## Limitations

- Assumes linear relationships  
- Reduces interpretability  
- Sensitive to feature scaling  
- May discard useful low-variance signals  

---

## Applications

- Data visualization  
- Feature extraction  
- Noise reduction  
- Image compression  
- Preprocessing for ML models  

---

## Evaluation Techniques

- Explained variance ratio  
- Reconstruction error  
- Visual inspection  

---

## Practical Considerations

- Always standardize features before PCA  
- Combine with clustering (K-Means, DBSCAN) for better results  
- Effective for high-dimensional datasets  
- Interpretation of components can be difficult  

---

## Implementation in This Repository

- PCA implementation  
- Dimensionality reduction visualization  
- Variance analysis  
- Integration with clustering algorithms  

---

## Repository Structure

PCA/

├── implementation notebooks  
├── experiments  
└── README.md  

---

## Key Takeaways

- PCA reduces dimensionality while preserving variance  
- Components are orthogonal and ranked by importance  
- Useful for preprocessing and visualization  
- Enhances performance of downstream models  

---

## References

- https://scikit-learn.org/stable/modules/decomposition.html#pca  
- https://developers.google.com/machine-learning/data-prep/transform/normalization  
- https://www.statlearning.com/  
- https://link.springer.com/book/10.1007/978-0-387-84858-7  
- https://www.ibm.com/topics/principal-component-analysis  

---
