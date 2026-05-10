# biomedFinal
This is the submission for Caleb Burton's 4116 Final Assignment. This includes the compiled Jupyter notebook file, report, and this README file.

# Explainable AI for Diabetic Retinopathy Classification

## Project Overview

This project builds an explainable AI pipeline for diabetic retinopathy severity classification using retinal fundus images.

The notebook trains a transfer learning model to classify images into one of five diabetic retinopathy severity levels:

- 0: No DR
- 1: Mild
- 2: Moderate
- 3: Severe
- 4: Proliferative DR

The project also includes explainability tools so the model output is easier to interpret.

## Main Notebook

The main project notebook is:

`biomedFinal.ipynb`

This notebook includes the full workflow:

- Dataset loading
- Image preprocessing
- Train, validation, and test split
- ResNet50 transfer learning model
- Two-stage training
- Model evaluation
- Confusion matrix
- ROC curves
- Grad-CAM visualization
- Occlusion sensitivity
- Groq-based explanation layer

## Dataset

This project uses the APTOS 2019 Blindness Detection dataset from Kaggle.

The notebook expects the dataset to be stored in Google Drive with this general structure:

```text
biomedFinal/
    dataset/
        train.csv
        train_images/
