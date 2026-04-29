# Neural Networks

<p align="center">
  <img src="https://purplegriffon.com/uploads/images/neural-network.png" width="600"/>
</p>

---

## Overview

**Neural Networks** are computational models inspired by the human brain, consisting of interconnected layers of neurons that process and transform data.

They are capable of learning **complex non-linear relationships** and form the foundation of modern **deep learning systems**.

---

## Objective

- Learn complex patterns from data  
- Model non-linear relationships  
- Perform classification and regression  
- Enable scalable learning across large datasets  

---

## What are Neural Networks?

Neural Networks consist of layers of connected neurons that transform inputs into outputs.

In simple terms:  
They learn by adjusting weights through repeated exposure to data.

---

## How It Works

1. Input data is passed to the network  
2. Each neuron computes a weighted sum  
3. Activation function is applied  
4. Output flows through layers  
5. Final prediction is generated  
6. Error is calculated  
7. Backpropagation updates weights  

Backpropagation computes gradients efficiently using the **chain rule** and updates weights to minimize loss. :contentReference[oaicite:0]{index=0}  

---

## Architecture

- **Input Layer** → Receives data  
- **Hidden Layers** → Extract features  
- **Output Layer** → Produces predictions  
- Fully connected (dense) structure  

---

## Formulas

### Neuron Computation

z = wᵀx + b  
a = φ(z)  

Where:  
- w → Weights  
- x → Input  
- b → Bias  
- φ → Activation function  

---

### Activation Functions

**Sigmoid**  
σ(z) = 1 / (1 + e^(−z))  

Derivative:  
σ'(z) = σ(z) · (1 − σ(z)) :contentReference[oaicite:1]{index=1}  

**ReLU**  
ReLU(z) = max(0, z)  

**Tanh**  
tanh(z) = (e^z − e^(−z)) / (e^z + e^(−z))  

Sigmoid maps values to a range between 0 and 1, enabling probabilistic outputs. :contentReference[oaicite:2]{index=2}  

---

### Loss Functions

**Mean Squared Error (Regression)**  
MSE = (1/n) Σ (yᵢ − ŷᵢ)²  

**Cross-Entropy (Classification)**  
J = −(1/n) Σ [y log(ŷ) + (1 − y) log(1 − ŷ)]  

---

### Backpropagation (Gradient Update)

w = w − α · ∂J/∂w  
b = b − α · ∂J/∂b  

Backpropagation computes gradients layer-by-layer using derivatives of activation functions. :contentReference[oaicite:3]{index=3}  

---

## Methodology

- Forward propagation through layers  
- Compute loss  
- Backpropagate error  
- Update weights using optimization  
- Iterate until convergence  

---

## Key Concepts

- Weights and biases control learning  
- Activation functions introduce non-linearity  
- Backpropagation enables training  
- Deep networks learn hierarchical features  

---

## Advantages

- Captures complex non-linear patterns  
- Highly flexible architecture  
- Scales well with large datasets  
- Backbone of modern AI systems  

---

## Limitations

- Requires large datasets  
- Computationally expensive  
- Sensitive to hyperparameters  
- Risk of overfitting  

---

## Applications

- Image recognition  
- Natural language processing  
- Speech recognition  
- Recommendation systems  
- Autonomous systems  

---

## References

- https://www.deeplearningbook.org/  
- https://scikit-learn.org/stable/modules/neural_networks_supervised.html  
- https://developers.google.com/machine-learning/crash-course  
- https://www.ibm.com/topics/neural-networks  
- https://en.wikipedia.org/wiki/Backpropagation  

---
