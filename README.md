# 🧠 Neural Networks From Scratch

This repository implements a neural network from the ground up using only `NumPy` and a lightweight spiral dataset generator from the `nnfs` python package. The goal is to gain a deeper understanding of what actually happens *under the hood* of popular deep learning frameworks like TensorFlow and PyTorch. While not exactly replicating, this implementation is highly instructive and offers full transparency into every component of neural network training.

---

## ✅ Implemented Features

### 🧩 Core Building Blocks
- **Dense (Fully Connected) Layer**  
  - Random initialization of weights and biases  
  - Forward pass: `output = X·W + b`  
  - Backward pass: gradient computation for weights, biases, and inputs

### 🔋 Activation Functions
- **ReLU (Rectified Linear Unit)**  
  - Forward pass: `max(0, x)`  
  - Backward pass: masks gradient where input <= 0  
- **Softmax**  
  - Converts logits to class probabilities  
  - Used for multi-class classification

### 📉 Loss Function
- **Categorical Cross-Entropy (CCE)**  
  - Works with both integer (sparse) labels and one-hot encoded labels  
  - Computes negative log-likelihood  
  - Suitable for multi-class classification problems

### 🔁 Training & Optimization
- Manual **forward and backward propagation**
- Basic **gradient descent** with **learning rate decay**
- Training on a **spiral dataset** generated using `nnfs`

---

## 🧪 Dataset
- **Spiral dataset**: A synthetic, non-linearly separable dataset with 3 classes — perfect for testing and visualizing neural networks. Generated using the `nnfs` python package.

---

## 💡 Motivation

This notebook is intended for educational purposes, helping to expose the internal mechanics of a neural network. Unlike high-level frameworks that abstract away many details, this implementation allows you to:

- Trace every step of forward and backward propagation
- Understand how gradients and updates are computed manually
- Visualize how neural networks learn from scratch

---

## 📦 Dependencies

```bash
pip install numpy nnfs
```

---

## 📁 Project Structure

```
Neural Networks From Scratch.ipynb  # Full implementation with step-by-step training and comments
```

---

## 🙋‍♂️ Notes

This project is a work in progress. Upcoming improvements include:
- Implementation of momentum in training neural networks
- Optimizers: ADAGRAD, RMSProp, ADAM
- Accuracy evaluation metrics
- L1/L2 Regularization methods and Dropout layers

---

Feel free to explore, modify, and build on this foundation to better understand how real neural networks function under the surface.
