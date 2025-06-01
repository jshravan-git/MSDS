
# Custom Neural Network

## 👨‍💻 Author  
**Saravanan Janarthanan**


---

## 📝 Project Summary

This project demonstrates the development and evaluation of a **custom-built feedforward neural network** applied to the **IRIS** and **MNIST** datasets. The objective is to understand core neural network mechanics, including forward/backward propagation and how custom components compare with established libraries like Keras and PyTorch.

---

## 🔧 Key Features

- Manual implementation of:
  - Dense layers
  - Activation functions (ReLU, Sigmoid, Softmax)
  - Loss functions (Cross-Entropy)
  - Batch Normalization
  - Dropout
- Gradient-based learning via custom backpropagation
- Comparison of performance with Keras and PyTorch models

---

## 📊 Datasets Used

### IRIS
- 150 samples, 4 features, 3 classes
- Goal: classify flower species

### MNIST
- 70,000 28×28 grayscale digit images
- Flattened into 784-length vectors
- Goal: classify digits from 0–9

---

## 🧮 Common Functions

### Activation Functions
- `sigmoid(x)`: maps input to (0, 1), used in binary classification
- `relu(x)`: sets negative values to 0
- `softmax(x)`: converts logits into probability distributions

### Derivatives
- `sigmoid_derivative(x)`
- `relu_derivative(x)`

### Loss Function
- `cross_entropy_loss(y_true, y_pred)`: used for multi-class classification

### Utility
- `one_hot_encode(y, num_classes)`: transforms labels to vector format

---

## 🧱 Neural Network Components

### Dense_Custom
Implements a fully connected layer with forward and backward methods using custom weight initialization and gradient updates.

### BatchNormalizationLayer_custom
Normalizes layer outputs during training using batch statistics, and applies learned `gamma` and `beta` scaling.

### DropoutLayer_custom
Randomly disables neurons during training to prevent overfitting; restores full connectivity during inference.

---

## 📈 Performance Evaluation

Models compared:
- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest
- XGBoost

**Best performer: XGBoost**
- Accuracy: 92%
- Precision: 90%
- F1 Score: 80%

---

## 🛠 Technologies Used

- Python
- NumPy, Pandas
- Matplotlib, Seaborn
- Jupyter Notebook

---

## ▶️ How to Run

1. Clone the repository or download the notebook.
2. Install required packages:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open the `.ipynb` file in Jupyter Notebook.
4. Run all cells in order to train models and visualize results.
