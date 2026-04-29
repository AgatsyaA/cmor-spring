# DBSCAN (Density-Based Spatial Clustering of Applications with Noise)

<p align="center">
  <img src="https://ik.imagekit.io/upgrad1/abroad-images/imageCompo/images/img_0_1_86GN1D.png" width="600"/>
</p>

---

## Overview

**DBSCAN** is a density-based unsupervised learning algorithm used to cluster data points based on **density connectivity**. It groups points that are closely packed together while identifying points in low-density regions as **noise (outliers)**.

Unlike centroid-based methods such as K-Means, DBSCAN does not require specifying the number of clusters in advance and can detect clusters of **arbitrary shapes**.

---

## Learning Objectives

- Understand density-based clustering principles  
- Learn how DBSCAN identifies clusters and outliers  
- Analyze the impact of ε (epsilon) and MinPts  
- Evaluate clustering performance and limitations  

---

## Problem Formulation

Given a dataset:

X = {x₁, x₂, ..., xₙ}

The objective is to partition the dataset into clusters such that:
- Points within a cluster are **density-connected**
- Sparse regions are identified as **noise**

---

## Key Concepts

### Core Points
A point x is a **core point** if:

|Nε(x)| ≥ MinPts

---

### Border Points
Points within the ε-neighborhood of a core point but not dense enough to be core points themselves.

---

### Noise Points (Outliers)
Points that are neither core nor border points.

---

### Density Reachability
A point y is directly reachable from x if:
- y ∈ Nε(x)  
- x is a core point  

---

### Density Connectivity
Two points are density-connected if there exists a chain of core points linking them.

---

## Parameters

### Epsilon (ε)
Defines the radius used to determine the neighborhood of a point.

---

### MinPts
Minimum number of points required to form a dense region.

Proper parameter selection is critical for model performance.

---

## Algorithm Workflow

1. Select an unvisited point  
2. Retrieve all points within ε  
3. If neighbors ≥ MinPts:
   - Mark as core point  
   - Create a new cluster  
   - Expand cluster via density reachability  
4. Else:
   - Mark as noise (may later become border)  
5. Repeat until all points are processed  

---

## Distance Metrics

- Euclidean Distance  
- Manhattan Distance  
- Cosine Distance  

Choice of metric significantly affects clustering results.

---

## Formulas

### ε-Neighborhood

Nε(x) = { y ∈ X | d(x, y) ≤ ε }

---

### Core Point Condition

|Nε(x)| ≥ MinPts

---

### Euclidean Distance

d(x, y) = √Σ (xᵢ − yᵢ)²  

---

### Silhouette Score

S = (b − a) / max(a, b)

Where:  
- a → Mean intra-cluster distance  
- b → Mean nearest-cluster distance  

---

## Advantages

- No need to specify number of clusters  
- Detects clusters of arbitrary shape  
- Robust to noise and outliers  
- Effective for spatial and density-based data  

---

## Limitations

- Sensitive to ε and MinPts  
- Struggles with varying density clusters  
- Performance degrades in high-dimensional spaces  
- Distance metric selection impacts results  

---

## Parameter Selection Strategy

- Use a **k-distance graph** to estimate ε  
- Set MinPts ≈ dimensionality + 1  
- Apply feature scaling before clustering  

---

## Applications

- Anomaly detection  
- Geospatial clustering  
- Customer segmentation  
- Image processing  
- Fraud detection  

---

## Evaluation Techniques

- Silhouette Score  
- Visual inspection  
- Cluster density validation  
- Domain-specific evaluation  

---

## Practical Considerations

- Feature scaling is essential for distance-based clustering  
- High dimensionality reduces effectiveness (curse of dimensionality)  
- PCA can improve clustering performance  
- Noise handling is a key advantage over centroid-based methods  

---

## Implementation in This Repository

- DBSCAN implementation  
- Parameter tuning experiments  
- Cluster and noise visualization  
- Comparison with other clustering methods  

---

## Repository Structure

DBSCAN/

├── implementation notebooks  
├── experiments  
└── README.md  

---

## Key Takeaways

- Clustering is based on **density, not centroids**  
- Automatically detects **outliers**  
- Works well for **irregular cluster shapes**  
- Requires careful parameter tuning  

---

## References

- https://scikit-learn.org/stable/modules/clustering.html#dbscan  
- https://developers.google.com/machine-learning/clustering/dbscan  
- https://www.statlearning.com/  
- https://link.springer.com/book/10.1007/978-0-387-84858-7  
- https://www.ibm.com/topics/dbscan  

---
