# Convolutional Neural Network (CNN) for Image Classification

## Introduction

This repository contains the implementation of a Convolutional Neural Network (CNN) using the Keras library with a TensorFlow backend. The primary goal of this model is image classification, making it suitable for tasks involving image analysis.

## Model Architecture

The CNN is designed with the following layers:

1. **Input Layer:**
   - Shape: Defined by `input_shape`
   - Represents the dimensions of the input images.

2. **Convolutional Layer (1):**
   - Filters: 8
   - Kernel Size: (3, 3)
   - Activation: ReLU
   - Learns features from the input images through convolution.

3. **Max Pooling Layer (1):**
   - Pool Size: (2, 2)
   - Reduces spatial dimensions, capturing essential information.

4. **Convolutional Layer (2):**
   - Filters: 16
   - Activation: ReLU
   - Another layer for feature extraction.

5. **Max Pooling Layer (2):**
   - Pool Size: (2, 2)
   - Further reduces spatial dimensions.

6. **Flatten Layer:**
   - Converts the 2D feature maps into a 1D vector.
   - Prepares the data for the fully connected layers.

7. **Dropout Layer:**
   - Rate: 0.5
   - Applies dropout regularization to reduce overfitting.

8. **Dense (Fully Connected) Output Layer:**
   - Units: `num_classes`
   - Activation: Softmax
   - Produces the final classification probabilities.

## Usage

1. **Requirements:**
   - TensorFlow
   - Keras

   Install dependencies using:
   ```bash
   pip install tensorflow
