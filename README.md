# Chest X-ray Classification Project

This repository contains the code and instructions for the final project of the Deep Learning Fundamentals Course (2024). The objective of the project is the classification of chest X-ray images to identify healthy individuals and those with pneumonia. The project also includes anomaly detection and explainability tasks.

## Project Overview

### Objective

Classification of chest X-ray images into:
1. Healthy
2. Bacterial Pneumonia
3. Viral Pneumonia

### Dataset

The Kaggle Chest X-ray Pneumonia Dataset, which contains 5,863 X-ray images divided into two main categories:
- Healthy
- With pneumonia (bacterial and viral)

The dataset is split into training, validation, and test sets. The test set is kept as is, while the training and validation sets can be combined and redistributed as needed.

### Tasks

1. **Binary Classification**: Healthy vs. Sick
2. **Multiclass Classification**: Healthy, Bacterial Pneumonia, Viral Pneumonia
3. **Anomaly Detection**: Identifying sick individuals with anomaly detection methods using only healthy data.
4. **Explainability**: Implementing and analyzing an explainability technique to understand model decisions.

## Prerequisites

### Step 1: Download Required Files

Download the model weights and KNN's joblib files from [Google Drive](https://drive.google.com/drive/folders/1gPmMeEmym7qc35gnU7JhfCrAPpwHjBZI).

### Step 2: Move Files to Your Google Drive

After downloading, move the files to a convenient location in your Google Drive.

### Step 3: Update Path Variables in the Notebook

Update the path variables in the test notebook to match the location of the downloaded files in your Drive.

Example paths to update:

```python
from pathlib import Path

BINARY_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/binary_model_VGG19_finetuned_weights_final.h5")
MULTICLASS_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/multiclass_model_ResNet101.keras")
ANOMALY_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/encoder_decoder_weights_final.h5")

BINARY_KNN_PATH = Path("/content/drive/MyDrive/chest_xray/binary_knn_classifier.joblib")
MULTI_KNN_PATH = Path("/content/drive/MyDrive/chest_xray/multi_knn_classifier.joblib")

```

## Notebooks

### Training Notebook

The training notebook includes:
- Data preprocessing and augmentation
- Model architectures for binary and multiclass classification
- Training procedures with transfer learning
- Saving the trained models

### Test Notebook

The test notebook allows you to:
- Load the pre-trained models
- Test the models on new X-ray images
- Perform anomaly detection
- Visualize the embedding vectors using t-SNE
- Apply explainability techniques to interpret model decisions
