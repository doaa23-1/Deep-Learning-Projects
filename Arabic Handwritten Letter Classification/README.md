# ✍️ Arabic Handwritten Letter Classification using CNN

This deep learning project focuses on building a convolutional neural network (CNN) to classify Arabic handwritten letters based on image data. The project tackles key challenges in Arabic handwriting recognition, including font variation, cursive writing, and personal handwriting differences.

---

## 🎯 Project Goal

To accurately classify 28 handwritten Arabic characters using a CNN model, and explore different hyperparameter tuning techniques to improve performance and reduce overfitting.

---

## 🧪 Dataset

- Source: El-Sawy et al. (2017) Arabic Handwritten Character Dataset
- Total images: 16,800 (28 classes)
- Participants: 60 individuals, aged 19–40
- Each letter written 10 times × 2 forms
- Split:
  - Training: 13,440 images
  - Testing: 3,360 images

---

## 🧠 Model Architecture

- 3 Convolutional layers (Conv2D) with ReLU activations
- 3 MaxPooling layers (2x2)
- Flatten layer
- Dense layer: 128 units with ReLU
- Dropout layer (rate: 0.5)
- Output Dense layer: 28 units with Softmax

---

## ⚙️ Training Setup

- Optimizer: Adam
- Epochs tested: 10, 15, 20
- Batch Sizes tested: 32, 64
- Best configuration:
  - Epochs: 15
  - Batch size: 64
  - Accuracy: **94.34%** on test set
  - No overfitting observed

---

## 🔬 Key Findings

- Increasing epochs improved accuracy until 15; beyond that, gains plateaued.
- Larger batch size helped stabilize training and reduce overfitting.
- CNNs are effective at capturing spatial features in handwritten Arabic letters.

---

## 👥 Team Members

- **Doaa Brnawi**  
- **Lamis Melebari**
- **Dania Salim**

---

## 🧾 Reference

> El-Sawy, A., Loey, M., & El-Bakry, H. (2017). Arabic Handwritten Characters Dataset.  
Used for training and evaluation purposes.

---

## 🧠 Tools & Technologies

- Python, Keras, TensorFlow
- Google Colab
- Matplotlib, NumPy
