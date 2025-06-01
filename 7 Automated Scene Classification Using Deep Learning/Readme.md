
# Automated Scene Classification Using Deep Learning

## 👨‍💻 Author  
**Saravanan Janarthanan**


---

## 📝 Project Summary

This project focuses on building a deep learning model for **automated scene classification** using image data. It aims to accurately categorize natural scenes—such as forests, mountains, and streets—into predefined categories using convolutional neural networks (CNNs) and transfer learning techniques.

The solution is designed to address the limitations of manual tagging by automating image categorization. It improves scalability, reduces human error, and supports real-time classification for applications like autonomous navigation, media management, and remote sensing.

---

## 🖼 Dataset Overview

The dataset is organized into folders for six scene categories:
- `buildings`, `forest`, `glacier`, `mountain`, `sea`, `street`

Each category is well-balanced across training and test sets:

| Dataset      | Class Range     | Notes                                |
|--------------|------------------|---------------------------------------|
| Training Set | ~2191 to 2512    | Balanced, with mountain most frequent |
| Test Set     | ~437 to 553      | Similar distribution as training set  |

**Image Format:**  
- Resized to 150×150 for CNN  
- Resized to 224×224 for MobileNet/ResNet

---

## 🧹 Data Preprocessing

Images are preprocessed using TensorFlow’s `ImageDataGenerator`:
- **Resizing** to required dimensions
- **Normalization** of pixel values to [0, 1]
- **Augmentation** (e.g., flipping, rotation) to enhance generalization

---

## 🧠 Model Overview

The project experiments with:
- **Custom CNN architecture**
- **Transfer learning** using:
  - MobileNetV2
  - ResNet50

Each model is trained and evaluated to compare performance in terms of accuracy, validation loss, and generalization.

---

## 📊 Evaluation Metrics
- Accuracy
- Validation accuracy/loss curves
- Confusion matrix (optional)

---

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- NumPy, Pandas
- Matplotlib / Seaborn
- Jupyter Notebook

---

## ▶️ How to Run

1. Clone the repository or download the notebook.
2. Install required packages:
   ```bash
   pip install tensorflow numpy pandas matplotlib seaborn
   ```
3. Ensure the image dataset is properly structured in training and test folders.
4. Open the notebook in Jupyter and run all cells sequentially to train and evaluate models.
