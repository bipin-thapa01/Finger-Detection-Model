# Finger Classification CNN Model

## About the Project
This project is a deep learning model built using **PyTorch**. 
The model learns to recognize the number of fingers shown in an image. It uses a **Convolutional Neural Network (CNN)**, which is a type of neural network specially designed for image processing tasks.

---

## What the Model Does
The model follows a clear 4-step pipeline:
1. Takes an image as input
2. Extracts important features from the image
3. Learns patterns during training
4. Predicts the number of fingers shown

---

## Main Components

### Dataset
The dataset contains images of fingers with corresponding labels.
* **Example:** Image of 3 fingers $\rightarrow$ Label = 3
* **Example:** Image of 5 fingers $\rightarrow$ Label = 5

### Image Processing
Before training, images undergo preprocessing to help the model learn better:
* Resized
* Rotated randomly
* Flipped randomly
* Converted into tensors

### CNN Layers
The CNN architecture contains:
* Convolution layers
* ReLU activation
* Max pooling
* Fully connected layers

These layers work together to help the model understand complex image patterns.

---

## How the CNN Works

```text
Input Image 
     ↓ 
Convolution Layer 
     ↓ 
    ReLU 
     ↓ 
Max Pooling 
     ↓ 
Convolution Layer 
     ↓ 
  Flatten 
     ↓ 
Fully Connected Layer 
     ↓ 
Output Prediction
