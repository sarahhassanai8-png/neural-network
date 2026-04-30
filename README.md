# neural-network
# 🧠 Neural Network Project - Heart Disease Prediction

## Project Overview

This project uses a Multilayer Perceptron (MLP) neural network to predict whether a patient has heart disease based on medical features.

---

## Dataset

* Name: Heart Disease Dataset
* Target:

  * 0 → No Heart Disease
  * 1 → Heart Disease
* Features include:

  * Age
  * Sex
  * Blood Pressure
  * Cholesterol
  * Chest Pain Type

---

##  Data Preprocessing

* Split data into:

  * Training set
  * Validation set
  * Testing set
* Applied StandardScaler for normalization
* Converted data into PyTorch tensors

---

##  Model Architecture

* Input Layer
* Hidden Layer 1: 32 neurons
* Hidden Layer 2: 16 neurons
* Output Layer: 1 neuron (Sigmoid)

### Techniques used:

* Batch Normalization
* Dropout

---

## Experiments

| Experiment | Activation | Accuracy |
| ---------- | ---------- | -------- |
| Exp 1      | ReLU       | 93.30%   |
| Exp 2      | Tanh       | 81.55%   |

---

## 📈 Results

* ReLU achieved higher accuracy than Tanh
* Faster training and better convergence with ReLU
* No overfitting observed

---

## 📊 Visualization

* Training Loss vs Validation Loss plotted in notebook

---

## 🚀How to Run

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Run the notebook:

```bash
jupyter notebook
```

3. Open:

```
notebook.ipynb
```

---

## 🏁 Conclusion

The ReLU activation function significantly improved performance compared to Tanh, making it the better choice for this classification task.
