**Handwritten Digit Recognition**
This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to recognize handwritten digits from the MNIST dataset. It trains a model, evaluates its accuracy, and provides functionality to capture and predict digits using a webcam interface.

**Features**
1.Uses MNIST dataset (60,000 training, 10,000 testing images)
2.Preprocessing and normalization of image data
3.CNN architecture for accurate classification
4.Live digit prediction via webcam using OpenCV and Google Colab JS integration
5.Model saving and loading with .h5 format

**Requirements**
Install the following dependencies (automatically handled in Colab):
bash
Copy
Edit
pip install opencv-python-headless
pip install tensorflow

**Model Architecture**
Conv2D (32 filters, 3x3) + ReLU + MaxPooling

Conv2D (64 filters, 3x3) + ReLU + MaxPooling

Conv2D (64 filters, 3x3) + ReLU

Flatten → Dense (64) → Dense (10, softmax)

**Training**
Optimizer: adam

Loss: sparse_categorical_crossentropy

Epochs: 5

Achieves ~99% accuracy on test data

**Live Prediction (Colab only)**
Uses webcam to draw and capture digits

Converts captured canvas to image

Predicts using the trained model in real-time

Files
Handwritten_Digit_Recognition.ipynb: Main Jupyter notebook with code and logic

digit_model.h5: Trained model saved after training

**Notes**
1.Works best in Google Colab
2.Webcam digit prediction might require multiple tries for accurate capture
3.You can extend this project with custom datasets or additional preprocessing
