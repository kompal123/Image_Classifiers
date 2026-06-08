# 🧬 Breast Cancer Histopathology Image Classification using Deep Learning

## Overview

This project implements and compares multiple deep learning approaches for **breast cancer histopathology image classification** using microscopic tissue images from the **BreaKHis dataset**. The objective is to automatically classify images into **benign** and **malignant** categories, demonstrating the application of artificial intelligence in medical image analysis.

The notebook includes data preprocessing, dataset preparation, model development, training, evaluation, and comparison of different neural network architectures.

---

## Models Implemented

### 1. Convolutional Neural Network (CNN)

A custom deep learning model built using TensorFlow/Keras for feature extraction and binary image classification.

### 2. Fully Connected Neural Network (FCNN)

A baseline dense neural network using flattened image inputs to compare performance against convolutional architectures.

### 3. Transfer Learning (VGG16)

A pre-trained VGG16 model is fine-tuned for breast cancer image classification, leveraging transfer learning to improve predictive performance.

---

## Dataset

The project uses the **BreaKHis (Breast Cancer Histopathological Image Classification)** dataset, containing microscopic images of benign and malignant breast tumors.

### Dataset classes

* Benign
* Malignant

Images are automatically divided into training and testing datasets before model training.

---

## Workflow

* Load and preprocess histopathology images
* Create train/test directory structure
* Generate image batches using `ImageDataGenerator`
* Train CNN model
* Train Fully Connected Neural Network
* Train VGG16 Transfer Learning model
* Evaluate model performance
* Generate confusion matrices and classification reports
* Compare classification accuracy across models

---

## Technologies Used

* Python
* TensorFlow / Keras
* PyTorch (dataset utilities)
* NumPy
* Matplotlib
* Scikit-learn
* OpenCV
* PIL
* tifffile

---

## Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* Classification Report

---

## Repository Structure

```text
├── Source_code
├── dataset/
│   ├── train/
│   │    ├── benign/
│   │    └── malignant/
│   └── test/
│        ├── benign/
│        └── malignant/
├── figures/
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Image-Classification.git
cd Image-Classification
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch the notebook:

```bash
jupyter notebook Image_classifiers.ipynb
```

---

## Key Learning Outcomes

* Medical image preprocessing
* Deep learning for image classification
* Transfer learning using VGG16
* Binary classification of histopathology images
* Performance evaluation of deep learning models
* Comparative analysis of CNN and transfer learning approaches

---

## Limitations

* Dataset paths are hardcoded and should be replaced with relative paths.
* Data preprocessing and model training are contained in a single notebook rather than modular scripts.
* Hyperparameter optimization and cross-validation are not included.
* Model checkpointing and early stopping can be added for improved training stability.

---

## Future Improvements

* Implement ResNet50, EfficientNet, and Vision Transformers (ViT)
* Add Grad-CAM for model explainability
* Perform hyperparameter optimization using Optuna
* Integrate MLflow for experiment tracking
* Deploy the trained model using Streamlit or FastAPI
* Containerize the project using Docker

---

## Author

**Kompal Fayyaz**

M.Sc. Bioinformatics
Freie Universität Berlin

**Research Interests**

* Bioinformatics
* Machine Learning
* Medical Image Analysis
* Computational Biology
* AI for Healthcare
* Deep Learning for Biomedical Applications

---

## License

This project is intended for educational and research purposes. Please ensure compliance with the original dataset licensing terms before redistribution or commercial use.
