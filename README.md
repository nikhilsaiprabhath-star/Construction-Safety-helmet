
# Construction Safety Helmet Detection Using CNN and Transfer Learning

## Project Overview

This project develops a deep learning-based image classification system to automatically detect whether a construction worker is wearing a safety helmet. The study compares the performance of a custom Convolutional Neural Network (CNN) with two transfer learning models, MobileNetV2 and ResNet50.

The project was developed as part of the Applied Machine Learning course at the University of Europe for Applied Sciences.

---

## Objectives

The main objectives of this project are:

- Develop a custom CNN model for helmet classification.
- Compare CNN performance with MobileNetV2 and ResNet50.
- Evaluate the impact of data augmentation techniques.
- Explain model predictions using Grad-CAM visualisations.
- Analyse model errors and misclassifications.

---

## Dataset Information

### Dataset Name
Project 01 – Helmet Classification Dataset

### Dataset Source
Roboflow Universe

### Dataset Link
https://universe.roboflow.com/project-xvwed/project-01-mj51m/dataset/1

### Dataset Summary

| Attribute | Value |
|------------|------------|
| Total Images | 2,886 |
| Classes | 2 |
| Training Images | 2,020 |
| Validation Images | 577 |
| Test Images | 289 |

### Classes

1. Helmet
2. No Helmet

---

## Research Questions

### RQ1 – Baseline Performance
What classification accuracy can a custom-designed CNN achieve on the Helmet / No-Helmet dataset without leveraging any pre-trained features?

### RQ2 – Transfer Learning Advantage
To what extent do pre-trained architectures (MobileNetV2 and ResNet50) outperform the custom CNN in accuracy, F1-score, and AUC when fine-tuned on this dataset?

### RQ3 – Model Interpretability
Which image regions does the best-performing model attend to when classifying helmet usage, as revealed by Grad-CAM visualisations?

### RQ4 – Data Augmentation Impact
How do standard augmentation techniques affect generalisation and reduce over-fitting?

### RQ5 – Error Characterisation
What are the dominant failure modes of each model, and what visual or contextual factors contribute to misclassifications?

---

## Models Used

### Custom CNN

The custom CNN architecture consists of:

- Conv2D Layers
- Batch Normalisation
- Max Pooling
- Dropout Layers
- GlobalAveragePooling2D
- Fully Connected Layers
- Sigmoid Output Layer

### Transfer Learning Models

- MobileNetV2
- ResNet50

Pre-trained ImageNet weights are used and fine-tuned on the helmet classification dataset.

---

## Data Preprocessing

The following preprocessing steps are applied:

- Image resizing (224 × 224)
- Pixel normalization
- Data augmentation:
  - Horizontal Flip
  - Rotation
  - Zoom
  - Width Shift
  - Height Shift
  - Brightness Adjustment

---

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix
- Classification Report

---


## Generated Outputs

### Figures

- Class Distribution Chart
- Sample Images Grid
- Data Augmentation Examples
- CNN Training Curves
- MobileNetV2 Training Curves
- ResNet50 Training Curves
- Confusion Matrices
- ROC Curves
- Grad-CAM Visualisations
- Error Analysis Images
- Model Comparison Charts

### Tables

- Dataset Summary
- CNN Architecture Summary
- Evaluation Metrics
- Model Comparison Table
- Error Analysis Table

---

## How to Run the Project

### Step 1: Clone Repository

```bash
git clone <repository-url>
```

### Step 2: Download Dataset

Download the dataset from:

https://universe.roboflow.com/project-xvwed/project-01-mj51m/dataset/1

### Step 3: Upload Dataset

Upload the dataset to Kaggle or place it in the project directory.

### Step 4: Open Notebook

Open:

```text
helmet_classification.ipynb
```

### Step 5: Run All Cells

Execute all notebook cells sequentially.

### Step 6: View Results

Generated figures and tables will be saved in:

```text
outputs/figures/
outputs/tables/
```

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- OpenCV
- Grad-CAM

---

## Author

**Nikhil Sai Prabhath Pinnaka**

MSc Program

University of Europe for Applied Sciences

Supervisor: Prof. Dr. Raja Hashim Ali
