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

[Dataset and saved models](https://drive.google.com/drive/folders/1E-rFggXe31DBS6GqPcflj2R_UQTpVbeY?usp=sharing) ...


“Download diabetic_data.csv from the UCI repository (https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008) or from the Drive folder (https://drive.google.com/drive/folders/1E-rFggXe31DBS6GqPcflj2R_UQTpVbeY?usp=sharing), and set DATA_PATH.

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

### Traditional Machine Learning

Logistic Regression: baseline classification model.

Random Forest Classifier: ensemble model for capturing nonlinear relationships.

LightGBM Classifier: gradient-boosting model for tabular data.

### Deep Learning

Feedforward Neural Network (Multilayer Perceptron): built using TensorFlow/Keras, with data input handled using tf.data.

## Evaluation Metrics

- Precision–Recall AUC (PR-AUC)

- ROC-AUC

- Macro-F1 Score

- Recall and Precision for the positive class (readmission within 30 days)

- Confusion Matrix
  

Model performance is compared to assess the trade-off between identifying patients at risk of early readmission and minimizing false-positive predictions.

## Project Links

- GitHub: https://github.com/Linda5-umwali/diabetes-readmission-prediction 
- Dataset and saved models: https://drive.google.com/drive/folders/1E-rFggXe31DBS6GqPcflj2R_UQTpVbeY?usp=sharing
- Demo video: https://www.loom.com/share/7d7121e0956c4c23b22cfdfb54b3cfa2
