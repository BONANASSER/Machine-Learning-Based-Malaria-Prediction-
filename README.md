# Machine-Learning-Based Malaria Prediction

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Healthy-green.svg)](https://example.com)
[![Docs](https://img.shields.io/badge/Docs-Updated-lightgreen.svg)](https://example.com/docs)

A concise, ML-driven prototype to predict malaria diagnosis using clinical and demographic features. The project aims to compare multiple algorithms, enhance performance via preprocessing (e.g., SMOTE), and identify influential clinical features to support decision-making in resource-limited settings.

---

## Overview

This project trains and evaluates multiple classifiers to predict malaria status from patient data. Core goals:

- Compare a diverse set of models (Decision Tree, Random Forest, ANN, SVM, KNN, Logistic Regression).
- Apply robust preprocessing: data cleaning, missing value handling, categorical encoding, normalization, and class-imbalance handling with SMOTE.
- Identify key predictive features to inform clinical decision support (top predictors include body temperature, travel history, and prior malaria infection history).
- Produce a compact, reproducible runbook and a ready-to-share README artifact.

Note: Reported accuracies in this repository are:
- Decision Tree: 100%
- Random Forest: 100%
- Artificial Neural Network (ANN): 99.09%
- Support Vector Machine (SVM): 94.54%
- K-Nearest Neighbor (KNN): 88.18%
- Logistic Regression: 85.45%

If you plan to publish, consider cross-validation details, data leakage checks, and a reproducibility narrative to accompany these results.

---

## Dataset

- Features (illustrative, non-exhaustive):
  - Age
  - Gender
  - Pregnancy status
  - Body temperature
  - Travel history
  - Previous malaria infection history
  - Other clinical/demographic indicators (e.g., symptoms, residence, exposure)

- Target:
  - Malaria status (positive/negative)

- Preprocessing highlights:
  - Data cleaning and imputation for missing values
  - Categorical encoding (e.g., one-hot encoding)
  - Feature normalization/scaling where appropriate
  - Addressing class imbalance with SMOTE
  - Train-test split for evaluation

---

## Models & Performance

A concise snapshot of model performance (on the same train-test split and preprocessing pipeline):

| Model | Accuracy (%) |
|---|---:|
| Decision Tree | 100.00 |
| Random Forest | 100.00 |
| Artificial Neural Network (ANN) | 99.09 |
| Support Vector Machine (SVM) | 94.54 |
| K-Nearest Neighbor (KNN) | 88.18 |
| Logistic Regression | 85.45 |

Notes:
- Perfect scores (100%) may indicate strong separability or potential data leakage; ensure a robust cross-validation strategy and clearly document evaluation methodology in the runbook.
- Feature importance (top predictors): Body temperature, Travel history, Previous malaria infection history.

---

## Feature Importance

Top predictors (based on the trained models and/or a feature importance method):

1. Body temperature
2. Travel history
3. Previous malaria infection history
4. [Other features as identified by your analysis]
5. [Additional features as identified by your analysis]

Interpretation (quick): Elevated body temperature is a classic malaria symptom; travel history relates to exposure risk; prior infection history may reflect susceptibility or observed exposure patterns. Use these insights to inform screening priorities and triage protocols.

---

## How to Run

Prerequisites:
- Python 3.x
- Virtual environment (recommended)
- Required packages installed from requirements.txt

1) Clone the repository
- git clone https://github.com/your-organization/Machine-Learning-Based-Malaria-Prediction.git
- cd Machine-Learning-Based-Malaria-Prediction

2) Create and activate a virtual environment
- Python 3.x must be installed on your system
- On macOS/Linux:
  - python3 -m venv venv
  - source venv/bin/activate
- On Windows:
  - python -m venv venv
  - venv\Scripts\activate

3) Install dependencies
- pip install -r requirements.txt

4) Run the main script
- python malaria_prediction.py

5) Expected outputs
- Trained model
  
#Results Summary (Concise)
Best-Performing Models (on reported test split): Decision Tree, Random Forest (100.00%); ANN (99.09%)
Other models: SVM (94.54%), KNN (88.18%), Logistic Regression (85.45%)
Top features: Body temperature, Travel history
