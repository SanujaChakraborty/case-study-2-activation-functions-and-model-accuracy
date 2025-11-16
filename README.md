# case-study-2-activation-functions-and-model-accuracy
Deep Learning Case Study: Activation Functions, their advantages/disadvantages, and methods to improve model accuracy.

# Case Study 2: Activation Functions & Methods to Improve Neural Network Accuracy

This repository contains the implementation and presentation for **Case Study 2** from my **M.Tech in AI & Data Science** coursework.

The goal of this study is to explore different activation functions used in neural networks, understand their strengths/limitations, and analyze how they affect model performance. The study also covers multiple techniques to improve accuracy in deep learning models.

---

## Repository Structure
```
/ppt/     → Presentation (Case Study 2 PPT)
/code/    → Notebook comparing activation functions
/data/    → Sample dataset used for demonstration
README.md → Summary of the case study
```

---

## 1. Introduction to Activation Functions

Activation functions introduce **non-linearity** in neural networks, enabling them to learn complex patterns.

### Why they matter:
```
- Help model non-linear relationships  
- Control gradient flow  
- Stabilize training  
- Affect convergence speed and performance  
```
---

## 2. Activation Functions Explored

The following activation functions were studied:

### **ReLU (Rectified Linear Unit)**
```
- Pros: Fast, avoids vanishing gradients  
- Cons: Dead neuron problem  
```
### **Leaky ReLU**
```
- Pros: Fixes the dead neuron issue  
- Cons: Slightly computationally heavier  
```
### **Sigmoid**
```
- Pros: Good for probabilities  
- Cons: Saturates, causes vanishing gradients  
```
### **Tanh**
```
- Pros: Zero-centered, smoother  
- Cons: Still suffers from vanishing gradients  
```
### **Softmax**
```
- Used in multi-class classification output layers  
```
---

## 3. Experimental Setup

We implemented simple neural network models using different activation functions:

1. **ReLU Model**
```
   - Hidden Layer: 7 neurons (ReLU)
   - Output Layer: 3 neurons (softmax)
```
2. **Leaky ReLU Model**
```
   - Hidden Layer: 7 neurons (Leaky ReLU)
   - Output Layer: softmax
```
3. **Sigmoid Model**
```
   - Hidden Layer: 7 neurons (sigmoid)
   - Output Layer: softmax
```
4. **Tanh Model**
```
   - Hidden Layer: 7 neurons (tanh)
   - Output Layer: softmax
```
---

## 4. Comparison of Results

### Key Observations:
```
- ReLU and Leaky ReLU performed best in terms of accuracy and convergence.
- Sigmoid and Tanh were slower due to gradient saturation.
- Softmax remained the best option for multi-class output.
```
The full result comparison is presented in the PPT.

---

## 5. Methods to Improve Model Accuracy

We experimented with the following optimization techniques:

### **Optimizers**
```
- Adam  
- RMSProp  
- SGD with momentum  
```
### **Loss Functions**
```
- Categorical Cross-Entropy  
- MSE  
```
### **Regularization & Stability Techniques**
```
- Batch Normalization  
- Dropout  
- Early Stopping  
```
### **Data Techniques**
```
- Data Augmentation  
- Hyperparameter tuning  
```
---

## 6. Insights & Recommendations
```
- Start with ReLU as the default activation function.
- Use Leaky ReLU when encountering dead neurons.
- Apply batch normalization for stability.
- Combine dropout + early stopping to prevent overfitting.
- Tune hyperparameters for optimal performance.
```
---

## Author
**Sanuja Chakraborty**  
M.Tech (AI & DS)

---

## Leave a star if you found this helpful!
