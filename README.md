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

## Installation Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/defungi.git
