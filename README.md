# Breast Cancer Histopathology Image Classification

## Overview

This project implements deep learning models for the classification of breast cancer histopathology images into **benign** and **malignant** categories using the **BreaKHis dataset**. The notebook explores different neural network architectures and transfer learning techniques to evaluate their performance on microscopic tissue images.

The project demonstrates an end-to-end image classification pipeline including dataset preprocessing, model training, evaluation, and visualization of classification performance.

---

## Features

* Histopathology image preprocessing
* Automatic dataset organization and train/test splitting
* Binary classification of breast cancer images
* Fully connected neural network baseline
* Transfer learning using **VGG16**
* Performance evaluation using confusion matrices and classification metrics
* Visualization of training and validation performance

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-learn
* Pandas
* Seaborn

---

## Dataset

The project uses the **BreaKHis (Breast Cancer Histopathological Database)** containing microscopic images of benign and malignant breast tumors at different magnification factors.

Dataset:
https://www.kaggle.com/datasets/ambarish/breakhis

---

## Workflow

1. Load and organize histopathology images
2. Split images into training and testing sets
3. Apply image preprocessing and augmentation
4. Train neural network models
5. Evaluate classification performance
6. Visualize confusion matrices and training curves

---

## Models Implemented

### Fully Connected Neural Network

* Flatten layer
* Dense (128)
* Dropout
* Dense (64)
* Sigmoid output

### Transfer Learning (VGG16)

* Pretrained VGG16 feature extractor
* Custom classification head
* Fine-tuning for breast cancer image classification

---

## Evaluation Metrics

* Accuracy
* Confusion Matrix
* Classification Report
* Training and Validation Loss
* Training and Validation Accuracy

---

## Future Improvements

* Implement ResNet50 and EfficientNet architectures
* Hyperparameter optimization using Optuna
* Explainability with Grad-CAM and SHAP
* Cross-validation
* Model deployment using Streamlit or FastAPI
* Docker containerization
* Experiment tracking with MLflow

---

## Repository Structure

```
├── Image_classifiers.ipynb
├── data/
├── models/
├── figures/
├── requirements.txt
└── README.md
```

---

## Installation

```bash
git clone <repository-url>

cd repository

pip install -r requirements.txt
```

---

## Run

Open the notebook:

```bash
jupyter notebook Image_classifiers.ipynb
```

or

```bash
jupyter lab
```

---

## Results

The project demonstrates the effectiveness of deep learning and transfer learning for automated breast cancer histopathology image classification and provides a reproducible workflow for biomedical image analysis.

---

## Author

**Kompal Fayyaz**

M.Sc. Bioinformatics
Freie Universität Berlin

Research Interests:

* Bioinformatics
* Machine Learning
* Computational Biology
* Medical Image Analysis
* AI for Healthcare
