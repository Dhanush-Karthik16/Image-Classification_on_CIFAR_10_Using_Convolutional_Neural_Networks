# 🧠 CIFAR-10 Image Classification using Convolutional Neural Networks

This project implements a **Convolutional Neural Network (CNN)** using **TensorFlow and Keras** to classify images from the **CIFAR-10 dataset**, a benchmark dataset for visual recognition tasks. The model is trained to recognize 10 classes of objects, such as airplanes, birds, trucks, and more.

---

## 📌 Project Overview

- **Dataset**: CIFAR-10 (available via `tensorflow.keras.datasets`)
- **Task**: Multi-Class Image Classification (10 categories)
- **Model Type**: Convolutional Neural Network (CNN)
- **Frameworks**: TensorFlow, Keras, NumPy, Matplotlib

---

## 📁 Dataset Description

The **CIFAR-10** dataset consists of:

- **60,000** color images (32x32 pixels)
- **10 classes**:  
  `airplane`, `automobile`, `bird`, `cat`, `deer`, `dog`, `frog`, `horse`, `ship`, `truck`
- Split into:
  - **50,000** training images
  - **10,000** test images

---

## 🧱 Model Architecture

```text
Input Layer     : 32x32 RGB images
Conv2D (32 filters, 3x3, ReLU)
MaxPooling2D
Conv2D (64 filters, 3x3, ReLU)
MaxPooling2D
Conv2D (64 filters, 3x3, ReLU)
Flatten
Dense (64 units, ReLU)
Dense (10 units, Output Layer, Softmax through logits)
