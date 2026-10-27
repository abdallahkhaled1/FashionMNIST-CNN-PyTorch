# FashionMNIST Image Classification with PyTorch 👗👟

This repository contains a Deep Learning project for classifying fashion items using a **Convolutional Neural Network (CNN)** built with **PyTorch**. The model is trained on the standard **FashionMNIST** dataset.

---

## 📌 Project Overview

The goal of this project is to build an end-to-end computer vision pipeline to categorize 28x28 grayscale images of clothing and shoes into 10 distinct classes.

- **Dataset:** FashionMNIST (60,000 training images, 10,000 test images)
- **Framework:** PyTorch
- **Hardware Acceleration:** CUDA (GPU)

---

## 🏗️ Model Architecture

The model (`FashionMNISTModel`) is a 2D Convolutional Neural Network consisting of:
1. **Conv2d Layer 1:** 1 in-channel, 10 out-channels, kernel size 3, stride 1, padding 1 + `ReLU` + `MaxPool2d`
2. **Conv2d Layer 2:** 10 in-channels, 10 out-channels, kernel size 3, stride 1, padding 1 + `ReLU` + `MaxPool2d`
3. **Flatten Layer:** Reshapes tensor to `(7 * 7 * 10 = 490)`
4. **Linear Layer:** Maps 490 features to 10 class outputs

---

## 📊 Results & Performance

- **Epochs:** 50
- **Batch Size:** 32
- **Optimizer:** Adam (`lr = 0.001`)
- **Loss Function:** CrossEntropyLoss
- **Test Accuracy:** **~89.87%**
- **Test Loss:** **~0.313**

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
   cd YOUR_REPOSITORY_NAME
