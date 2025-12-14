🧠 MNIST Digit Classification using Convolutional Neural Networks (CNN)

This project presents an end-to-end implementation of a Convolutional Neural Network (CNN) for classifying handwritten digits (0–9) using the MNIST dataset.
The model is built using TensorFlow/Keras and achieves high accuracy with strong generalization performance.

📌 Project Overview

Handwritten digit recognition is a classic problem in computer vision and deep learning.
In this project, a CNN model is designed, trained, and evaluated to accurately classify digits from grayscale images of size 28×28.

The project covers the complete workflow:

Data loading and preprocessing

CNN architecture design

Model training and regularization

Performance evaluation

Visualization of results

🚀 Key Features

Data normalization and reshaping

CNN architecture with convolution, pooling, and dropout layers

Early stopping to prevent overfitting

Model checkpointing (saving best model)

Confusion matrix visualization

Sample prediction visualization

Clean and modular project structure

🧠 Model Architecture

The CNN architecture consists of:

Conv2D (32 filters) with ReLU activation

Conv2D (64 filters) with ReLU activation

MaxPooling2D for spatial downsampling

Dropout for regularization

Fully Connected (Dense) layers

Softmax output layer for multi-class classification

This design allows the model to extract low-level and high-level features efficiently.

📊 Model Performance
Metric	Value
Training Accuracy	~98.9%
Validation Accuracy	~99.0%
Test Accuracy	~98.88%
Test Loss	~0.033

The model demonstrates excellent generalization with no significant overfitting.

📂 Project Structure
mnist-cnn-digit-classification/
│
├── model/
│   └── mnist_cnn_model.h5
│
├── src/
│   └── train.py
│
├── examples/
│   ├── confusion_matrix.png
│   └── sample_predictions.png
│
├── README.md
└── requirements.txt

▶️ How to Run the Project
1️⃣ Install dependencies
pip install -r requirements.txt

2️⃣ Train the model
python src/train.py


The trained model will be saved in the model/ directory and evaluation figures will be stored in examples/.

🛠️ Technologies Used

Python

TensorFlow / Keras

NumPy

Matplotlib

Seaborn

Scikit-learn

🎯 Future Improvements

Data augmentation for improved robustness

Batch normalization layers

Hyperparameter tuning

Deployment using a web interface (Streamlit or Flask)

✨ Author

Developed by Doaa Brnawi
Deep Learning Projects Repository
