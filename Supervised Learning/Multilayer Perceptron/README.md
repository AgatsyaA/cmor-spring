# Multilayer Perceptron (MLP)

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/4/46/Colored_neural_network.svg" width="600"/>
</p>

---

## Overview

A **Multilayer Perceptron (MLP)** is a class of **feedforward artificial neural networks** consisting of multiple layers of neurons. It is capable of learning **complex non-linear relationships** between inputs and outputs.

MLPs extend simple linear models by introducing **hidden layers and non-linear activation functions**, making them powerful for both classification and regression tasks.

---

## Objective

- Learn complex non-linear mappings  
- Model high-dimensional relationships  
- Perform classification and regression  
- Enable deep learning-based predictions  

---

## What is an MLP?

An MLP consists of:

- **Input Layer** → Receives features  
- **Hidden Layers** → Perform transformations  
- **Output Layer** → Produces predictions  

In simple terms:  
An MLP learns by passing data through layers of weighted connections and applying non-linear transformations.

---

## How It Works

1. Input data is fed into the network  
2. Each neuron computes a weighted sum  
3. Activation function is applied  
4. Output is passed to the next layer  
5. Final prediction is generated  
6. Errors are propagated backward (backpropagation)  
7. Weights are updated using optimization  

---

## Architecture

- Fully connected layers (dense layers)  
- Multiple hidden layers  
- Non-linear activation functions  
- Feedforward data flow  

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

**ReLU**  
ReLU(z) = max(0, z)  

**Tanh**  
tanh(z) = (e^z − e^(−z)) / (e^z + e^(−z))  

---

### Loss Function (Example: MSE)

MSE = (1/n) Σ (yᵢ − ŷᵢ)²  

For classification, cross-entropy is commonly used.

---

### Backpropagation (Gradient Update)

w = w − α · ∂J/∂w  

b = b − α · ∂J/∂b  

Where:  
- α → Learning rate  
- J → Loss function  

---

## Methodology

- Forward propagation through layers  
- Compute loss  
- Backpropagate gradients  
- Update weights using optimization  
- Repeat until convergence  

---

## Key Concepts

- Hidden layers enable non-linearity  
- Activation functions introduce complexity  
- Backpropagation enables learning  
- Overfitting controlled via regularization  

---

## Advantages

- Captures complex non-linear relationships  
- Flexible architecture  
- Applicable to a wide range of problems  
- Forms the basis of deep learning  

---

## Limitations

- Requires large datasets  
- Computationally expensive  
- Sensitive to hyperparameters  
- Can overfit without regularization  

---

## Applications

- Image classification  
- Natural language processing  
- Speech recognition  
- Recommendation systems  
- Time-series forecasting  

---

## References

- https://scikit-learn.org/stable/modules/neural_networks_supervised.html  
- https://www.deeplearningbook.org/  
- https://developers.google.com/machine-learning/crash-course  
- https://www.ibm.com/topics/neural-networks  
- https://link.springer.com/book/10.1007/978-0-387-84858-7  

---
