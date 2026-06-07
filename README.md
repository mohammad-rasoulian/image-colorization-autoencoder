
# Image Colorization using Convolutional Autoencoder

A deep learning project for converting grayscale images into color images using a convolutional autoencoder built with TensorFlow and Keras.

This project uses the CIFAR-10 dataset to train a neural network that receives grayscale images as input and reconstructs their RGB color versions.

---

## Overview

Image colorization is a computer vision task where a model learns to predict color information from grayscale images.

In this project, a convolutional encoder-decoder architecture is trained to reconstruct color images from grayscale inputs.

The model learns visual patterns from CIFAR-10 images and generates approximate colorized outputs.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- CIFAR-10 Dataset

---

## Model Architecture

The model is based on a convolutional autoencoder:

### Encoder

- Conv2D layers
- ReLU activation
- MaxPooling layers

### Decoder

- Conv2D layers
- ReLU activation
- UpSampling layers
- Final Conv2D layer with sigmoid activation

---

## Workflow

1. Load CIFAR-10 dataset
2. Normalize RGB images
3. Convert RGB images to grayscale
4. Build convolutional autoencoder
5. Train model using Mean Squared Error loss
6. Predict color images from grayscale inputs
7. Compare grayscale input, model prediction, and original image

---

## Results

The model generates colorized versions of grayscale CIFAR-10 images.

Recommended screenshot:

```text
screenshots/sample_predictions.png
