# 🧠 Neural Network Project - Heart Disease Prediction

## 📌 Project Overview

This project uses a Multilayer Perceptron (MLP) Neural Network built with PyTorch to predict whether a patient has heart disease based on medical features from a heart disease dataset.

The project compares two activation functions:
- ReLU
- Tanh

to determine which one provides better performance for binary classification.

---

# 📂 Dataset

| Item | Description |
|---|---|
| Dataset Name | Heart Disease Dataset |
| File Name | Heart_disease - Heart_disease.csv |
| Problem Type | Binary Classification |
| Target Column | target |

### 🎯 Target Values

| Value | Meaning |
|---|---|
| 0 | No Heart Disease |
| 1 | Heart Disease |

### Features Include

- Age
- Sex
- Blood Pressure
- Cholesterol
- Chest Pain Type
- Maximum Heart Rate
- Exercise Induced Angina
- And other medical attributes

---

# ⚙️ Data Preprocessing

The following preprocessing steps were applied:

- Splitting dataset into:
  - Training Set
  - Validation Set
  - Testing Set

- Applying feature scaling using StandardScaler()

- Converting data into PyTorch tensors

- Checking missing values in the dataset

---

# 🧠 Model Architecture

The Neural Network architecture consists of:

| Layer | Details |
|---|---|
| Input Layer | Number of input features |
| Hidden Layer 1 | 32 neurons |
| Hidden Layer 2 | 16 neurons |
| Output Layer | 1 neuron with Sigmoid activation |

---

# 🔬 Techniques Used

| Technique | Purpose |
|---|---|
| Batch Normalization | Improves training stability |
| Dropout (0.3) | Prevents overfitting |
| Early Stopping | Stops training when validation loss stops improving |
| Learning Rate Scheduler | Reduces learning rate during training |

---

# 🧪 Experiments

| Experiment | Activation Function | Accuracy |
|---|---|---|
| Experiment 1 | ReLU | 93.30% |
| Experiment 2 | Tanh | 81.55% |

---

# 📈 Results

## ReLU Activation

Formula:

f(x) = max(0, x)

### Advantages

- Faster convergence
- Better performance
- Reduced vanishing gradient problem

---

## Tanh Activation

Formula:

tanh(x) = (e^x - e^-x) / (e^x + e^-x)

### Observations

- Slower training
- Lower accuracy compared to ReLU

---

# 📊 Visualizations

The notebook includes several visualizations:

- Training Loss Curve
- Validation Loss Curve
- ReLU vs Tanh Comparison
- Final Accuracy Comparison

These plots help evaluate:
- Model learning behavior
- Overfitting
- Generalization performance

---

# 🚀 How to Run

## 1️⃣ Install Dependencies
pip install -r requirements.txt

## 2️⃣ Run Jupyter Notebook
jupyter notebook

## 3️⃣ Open Notebook
notebook.ipynb

---

# 📦 Libraries Used

- PyTorch
- Pandas
- Matplotlib
- Scikit-learn

---

# 🏁 Conclusion

This project demonstrates how Deep Learning can be applied to medical diagnosis problems using Neural Networks.

The comparison between ReLU and Tanh activation functions showed that:

- ReLU achieved higher accuracy
- ReLU provided faster convergence
- ReLU reduced training issues such as vanishing gradients

Therefore, ReLU was the better activation function for this heart disease classification task.
