# Handwritten Digit Recognition with CNN and Pygame Interface

This project demonstrates a deep learning pipeline that recognizes handwritten digits using a Convolutional Neural Network (CNN) trained on the MNIST dataset, and provides a real-time digit recognition interface using Pygame.

## 📌 Features

- Train a CNN model on the MNIST dataset using Keras.
- Save the best-performing model using `ModelCheckpoint`.
- Real-time handwritten digit input using Pygame.
- Instant digit prediction from the GUI using the trained model.

---

## 🧠 Model Training (`digit.ipynb`)

- Dataset: [MNIST Handwritten Digits](http://yann.lecun.com/exdb/mnist/)
- Model Architecture:
  - Convolutional Layers (`Conv2D`)
  - Pooling Layers (`MaxPool2D`)
  - Dropout for regularization
  - Dense output with `softmax` activation
- Training Enhancements:
  - EarlyStopping and ModelCheckpoint callbacks
  - Validation split to monitor performance
- Output:
  - A `.keras` model file (e.g., `bestmodel.keras`)

---

## 🎨 Digit Prediction App (`app.py`)

- Built using `pygame` and `OpenCV`.
- Features:
  - Draw digits on a 640x480 canvas.
  - Real-time digit recognition on mouse release.
  - Clear canvas with `"n"` key.
- Predictions are displayed on the canvas using a red label.

