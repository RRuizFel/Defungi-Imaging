# Defungi Dataset and Code

This repository contains the code for processing and analyzing the **Defungi** dataset. The dataset consists of images of various fungal species, and the code includes functionalities for feature extraction, dataset creation, and machine learning model evaluation. The models implemented are **Random Forest** and **MLP (Multi-layer Perceptron)**, with comparisons between standard and PCA-based versions of each model.

## Table of Contents
- [Project Overview](#project-overview)
- [Installation Instructions](#installation-instructions)
- [Dataset Description](#dataset-description)
- [Code Functionality](#code-functionality)
  - [Image Preprocessing](#image-preprocessing)
  - [Feature Extraction](#feature-extraction)
  - [Model Training and Evaluation](#model-training-and-evaluation)
  - [Model Comparison](#model-comparison)
  - [Confusion Matrix and ROC Curve](#confusion-matrix-and-roc-curve)
- [Results and Performance](#results-and-performance)
- [License](#license)

## Project Overview

This project aims to classify fungal species based on their image features using machine learning techniques. It includes:
- Feature extraction techniques such as color histograms, GLCM (Gray Level Co-occurrence Matrix), and Local Binary Patterns (LBP).
- Dimensionality reduction using **PCA (Principal Component Analysis)**.
- Classification using machine learning models like **Random Forest**, **MLP**, and their PCA-based versions.
- Evaluation using metrics such as accuracy, precision, recall, F1-score, confusion matrix, and ROC curve.

## Dataset Description

The **Defungi** dataset contains images of various species of fungi. The images are organized into subdirectories, with each subdirectory representing a different fungal species. The dataset supports `.jpg`, `.jpeg`, and `.png` image formats.

## Installation Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/defungi.git

## Code Functionality

### Image Preprocessing
The dataset's images are preprocessed to extract features relevant for classification tasks. Preprocessing steps include:

- **Resizing** images to a fixed size (64x64).
- **Color space transformation:** Convert images to HSV and LAB color spaces.
- **Grayscale conversion:** For texture feature extraction.

### Feature Extraction
The following features are extracted from each image:

1. **Color Histograms:** Histogram in HSV and LAB color spaces.
2. **Texture Features:** Extracted using GLCM (Gray Level Co-occurrence Matrix) for properties like contrast, dissimilarity, homogeneity, energy, and correlation.
3. **Local Binary Patterns (LBP)**: A method for texture analysis.
4. **Average Intensity:** The average pixel intensity in grayscale.

### Model Training and Evaluation
The features extracted from images are used to train machine learning models:

- **Random Forest Classifier.**
- **MLP Classifier.**

For each model, the following evaluation metrics are computed:
- Accuracy
- Precision
- Recall
- F1 Score

### Model Comparison
The project compares different models:

- **Random Forest vs. PCA Random Forest.**
- **MLP vs. PCA MLP**.

Performance metrics (accuracy, precision, recall, and F1 score) are visualized using bar charts for easy comparison.

### Confusion Matrix and ROC Curve
- **Confusion Matrix:** For each model, a confusion matrix is plotted to visually evaluate classification performance.
- **ROC Curve:** The Receiver Operating Characteristic (ROC) curve is plotted for each model, displaying how well the model distinguishes between classes.

## Results and Performance
The project evaluates the performance of the machine learning models using different configurations. The following results are reported:
- Model accuracy, precision, recall, and F1 score for both **Random Forest and MLP** classifiers.
- Comparison of models based on their performance metrics (e.g., confusion matrix and ROC curve).
