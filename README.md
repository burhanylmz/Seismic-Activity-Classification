# Seismic Activity Detection with Deep Learning (PyTorch)

This project implements a non-linear binary classification model using **PyTorch** to detect seismic events based on underground wave energy and vibration axis variation. The model effectively handles non-linearly separable data to achieve high precision.

[Image of binary classification decision boundary]

## 🚀 Performance Highlights
* **Test Accuracy:** ~99.00%
* **Loss Reduction:** Successfully converged from a starting MSE loss to ~0.37.
* **Generalization:** No signs of overfitting; training and test loss remained closely aligned throughout the process.

## 🧠 Model Architecture
The model uses a Multi-Layer Perceptron (MLP) architecture designed to solve complex decision boundaries that a simple linear model cannot address.

* **Input Layer:** 2 features (Wave Energy, Vibration Variation).
* **Hidden Layer:** 10 neurons with **ReLU** activation to introduce non-linearity.
* **Output Layer:** 1 neuron (Logit output for binary classification).

[Image of a neural network with one hidden layer and ReLU activation]

## ⚙️ Hyperparameters & Optimization
* **Loss Function:** `BCEWithLogitsLoss` (chosen for numerical stability and handling sigmoid internally).
* **Optimizer:** `Adam` (Adaptive Moment Estimation) with a learning rate of 0.01 for faster and more stable convergence compared to standard SGD.
* **Epochs:** 160.

[Image of Adam optimizer vs SGD convergence]

## 🛠️ Tech Stack
* **Framework:** PyTorch
* **Data Handling:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab

## 📂 Project Structure
* `kod2.ipynb`: Full implementation of the data preprocessing, model definition, and training loop.
* `08-seismic_activity_svm.csv`: The dataset containing seismic features and labels.

---
**Developed by Burhan Yılmaz** *Software Engineering Student at Aksaray University*
