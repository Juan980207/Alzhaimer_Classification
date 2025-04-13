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

## Results Summary

| Model            | Accuracy | Precision | Recall | PSNR   | SSIM  |
|------------------|----------|-----------|--------|--------|-------|
| ResNet50         | 0.88     | 0.88      | 0.88   |   -    |   -   |
| Custom CNN       | 0.88     | 0.88      | 0.88   |   -    |   -   |
| Residual U-Net   |   -      |    -      |   -    | 30.21  | 0.922 |
| Ensemble Model   | 0.82     | 0.82      | 0.82   |   -    |   -   |

 Residual U-Net was the best denoising model.  
 Ensemble model improved recall by +0.21 pts on noisy images.

## Dataset

MRI data used from the [OASIS dataset (2009)](https://www.oasis-brains.org/), consisting of ~80,000 anonymized brain MRI slices, labeled into four dementia classes:
- Non-demented
- Very mild
- Mild
- Demented

> Dataset was balanced by sampling the same number of images per class.

##  Research Goals

- Evaluate how denoising affects CNN-based classification performance
- Compare custom-built CNNs with transfer learning models
- Explore the effectiveness of an ensemble approach for real-world noisy MRI images

##  Author

Juan Manuel González Rincón
MSc Data Science | University of Hertfordshire
