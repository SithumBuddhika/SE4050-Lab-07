# SE4050 – Deep Learning Lab 07

## Autoencoders

**Student Name:** Sithum Buddhika Jayalal  
**Registration Number:** IT23177482  
**Module:** SE4050 – Deep Learning  

## Overview

This repository contains the implementations completed for Deep Learning Lab 07.

The lab focuses on Autoencoders using the Fashion-MNIST dataset and includes three different implementations:

1. Feed-Forward Neural Network Autoencoder
2. Vanilla CNN Autoencoder
3. CNN Image Denoising Autoencoder

Each model was trained for 30 epochs and evaluated using Mean Squared Error (MSE).

## Implementations

### 1. FFNN Autoencoder

A dense-layer-based autoencoder was used to reconstruct Fashion-MNIST images.

**Test MSE:** approximately `0.008615`

The model compresses each image into a latent representation and reconstructs the image using dense layers.

### 2. Vanilla CNN Autoencoder

A convolutional autoencoder was implemented using Conv2D and Conv2DTranspose layers.

**Test MSE:** approximately `0.001808`

The CNN Autoencoder achieved better reconstruction performance than the FFNN Autoencoder because convolutional layers preserve spatial information in images.

### 3. CNN Image Denoising Autoencoder

Noise was added to Fashion-MNIST images and a CNN-based autoencoder was trained to reconstruct the original clean images.

**Noise Factor:** `0.2`

**Test MSE:** approximately `0.006501`

The model successfully reduced noise while preserving the main structure of the original images.

## Model Comparison

| Model | Test MSE |
|---|---:|
| FFNN Autoencoder | 0.008615 |
| Vanilla CNN Autoencoder | 0.001808 |
| CNN Denoising Autoencoder | 0.006501 |

The Vanilla CNN Autoencoder achieved the lowest reconstruction error for clean image reconstruction.

The Denoising Autoencoder performs a more difficult task because it reconstructs clean images from noisy inputs.

## Key Concepts

This lab covered:

- Autoencoders
- Encoder and Decoder architectures
- Latent representations
- Image reconstruction
- Convolutional Autoencoders
- Image denoising
- Mean Squared Error
- Linear Autoencoders and PCA
- Autoencoders vs Variational Autoencoders

## Files

- `lab_7_AE_FFNN.ipynb` – Feed-Forward Autoencoder
- `lab_7_AE_Vanilla_CNN.ipynb` – Vanilla CNN Autoencoder
- `lab_7_AE_CNN_Image_Denoising.ipynb` – CNN Denoising Autoencoder
- `IT23177482.pdf` – Lab 07 report

## Tools and Technologies

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Google Colab
- Fashion-MNIST

## Author

**Sithum Buddhika Jayalal**  
**IT23177482**
