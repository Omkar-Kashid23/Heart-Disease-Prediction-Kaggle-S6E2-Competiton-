# Heart Disease Prediction (Kaggle S6E2)

This repository contains a high-performance machine learning solution for predicting the presence of heart disease using clinical data. The model is trained on a massive dataset of **630,000 records**, achieving a robust **ROC-AUC score of 0.9555** through rigorous cross-validation.

## 📌 Project Overview

The goal of this project is to develop a binary classification system that accurately identifies heart disease based on several patient clinical parameters.

### Key Features:

* **Large-Scale Data Handling**: Optimized for a dataset with over half a million training samples.
* **Automated Preprocessing**: Includes comprehensive one-hot encoding and feature scaling.
* **Robust Validation**: Utilizes 5-fold cross-validation to ensure model stability and generalization.

## 🛠️ Tech Stack

* **Language**: Python
* **Libraries**:
* `pandas` & `numpy` for data manipulation
* `scikit-learn` for model building, scaling, and evaluation


* **Model**: Logistic Regression

## 📊 Dataset Description

The model utilizes 14 clinical features, including:

* **Demographics**: Age, Sex.
* **Clinical Measurements**: BP, Cholesterol, Max HR, ST depression.
* **Diagnostic Indicators**: Chest pain type, EKG results, Thallium.

## ⚙️ Workflow

1. **Data Cleaning**: Verified zero null values across 630k rows.
2. **Feature Engineering**: Applied **One-Hot Encoding**, expanding the feature space to **453 columns** to capture categorical relationships.
3. **Scaling**: Used `StandardScaler` to normalize features for faster Logistic Regression convergence.
4. **Training**: Implemented **Logistic Regression** with a maximum of 1,000 iterations.
5. **Evaluation**: Used **5-Fold K-Fold Cross-Validation** with ROC-AUC as the primary metric.

## 📈 Model Performance

| Metric | Score |
| --- | --- |
| **Mean CV ROC-AUC** | **0.9555** |
| **Fold Consistency** | 0.9548 - 0.9560 |

## 🚀 How to Run

1. Clone the repository.
2. Install dependencies: `pip install pandas scikit-learn numpy`.
3. Run the notebook `Kaggle(S6E2).ipynb`.
