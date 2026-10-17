# diabetes-readmission-prediction
## Overview

This project investigates whether machine learning and deep learning
models can predict 30-day hospital readmission among patients with
diabetes using the Diabetes 130-US Hospitals dataset.

The target is binary:
- `1`: Readmitted within 30 days (`<30`)
- `0`: Not readmitted within 30 days (`NO`) or readmitted after 30 days (`>30`)

The project also examines model performance across age groups, race
categories, and insulin status to identify potential differences in
predictive performance.

## Research Objectives

- Develop a model to predict 30-day readmission.
- Compare traditional machine learning models with a neural network.
- Evaluate models using PR-AUC, macro-F1, and positive-class recall.
- Investigate performance differences across patient subgroups.
- Document experiments and limitations to support reproducibility.

## Dataset

The project uses the Diabetes 130-US Hospitals dataset.

The raw dataset is not included in this repository. Obtain it from
the original dataset source or the linked project data folder.

[Dataset and saved models](GOOGLE_DRIVE_LINK) ...

## Methodology

1. Data loading and quality checks.
2. Data cleaning and feature preprocessing.
3. Patient-level train, validation, and test splitting.
4. Training and comparison of traditional ML and deep learning models.
5. Hyperparameter experiments and class-imbalance handling.
6. Model selection using validation data.
7. Final test evaluation and subgroup analysis.

Patient identifiers are used to prevent encounters belonging to the
same patient from appearing in different splits, and are excluded
from the predictive features.

## Models

Update this list to reflect the models actually trained:
- Logistic Regression
- Random Forest
- Gradient Boosting
- TensorFlow/Keras neural network

## Evaluation Metrics

- PR-AUC (Average Precision)
- Macro-F1 score
- Recall for the positive class
- Confusion matrix
- ROC-AUC, where appropriate

## Project Links

- GitHub: https://github.com/Linda5-umwali/diabetes-readmission-prediction 
- Dataset and saved models: 
- Demo video:
