# Alzheimer's Disease Classification from MRI using CNN and U-Net

This project aims to improve the classification of Alzheimer's disease stages by combining advanced image denoising techniques (U-Net architectures) with convolutional neural networks (CNNs). The model processes noisy MRI brain scans and classifies them into different levels of dementia severity.

## Project Overview

Accurate and early detection of Alzheimer's disease is key for improving patient outcomes. This study investigates how preprocessing noisy MRI images using various denoising models enhances the performance of deep learning classifiers.

### Key Features

- MRI image denoising using:
  - Autoencoder
  - Classic U-Net
  - Residual U-Net
- Alzheimer's classification using:
  - Custom CNN
  - ResNet50 (transfer learning)
- Ensemble model combining Residual U-Net + Custom CNN
- Evaluation with metrics: Accuracy, Precision, Recall, PSNR, SSIM

## Technologies Used

- Python 3.x
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib
- Scikit-learn
- Jupyter Notebooks

## Project Structure
