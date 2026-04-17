# Multi-Label Medical Imaging AI Classification System

## Overview

This project implements a complete deep learning pipeline for multi-label classification of medical images, focusing on detecting multiple pathological findings within a single image.

The system is designed to process medical imaging datasets (e.g., chest X-rays) and predict multiple co-existing conditions using convolutional neural networks.


## Problem Statement

In medical imaging, a single scan can contain multiple pathologies simultaneously.

Unlike traditional classification tasks, this project addresses:
- **Multi-label classification** (not mutually exclusive classes)
- **Class imbalance**
- **Medical data variability**


## Pipeline Overview

The system includes a full end-to-end workflow:

1. Data preprocessing
2. Dataset balancing & augmentation
3. Train/test split
4. Model training
5. Model evaluation
6. Inference & prediction


## Dataset
Source: NIH Chest X-ray Dataset (Kaggle)
Contains:
Thousands of labeled X-ray images
Multiple disease annotations per image

Each image can belong to multiple classes simultaneously


## Data Processing

The pipeline includes:

Image resizing and normalization
Removal of unwanted classes
Dataset balancing:
Class reduction
Targeted augmentation
Statistical analysis of label distribution


## Data Augmentation

To address class imbalance:

Class-specific augmentation
Synthetic data generation
Controlled reduction of dominant classes

Improves generalization and model robustness


## Model

Convolutional Neural Networks (CNN)
Multi-label output (sigmoid activation)
Loss function: Binary Cross-Entropy
Architectures:
- Custom CNN
- ResNet-based model (for comparison)


## Training

Multi-label classification setup
Train/test split
Evaluation based on:
Precision / Recall
Class-wise performance
Dataset statistics


## Inference

The system supports:

Single image prediction
Batch prediction
Full dataset inference
python 5_multi_label_classification_predict.py


## Deployment
Models exported to TensorFlow.js
Enables:
Web-based inference
Lightweight deployment


## Use Cases
Automated radiology support tools
Multi-pathology detection systems
Medical AI research pipelines
Clinical decision support systems

##  Disclaimer

This project is for research purposes only and does not replace medical diagnosis by healthcare professionals.

