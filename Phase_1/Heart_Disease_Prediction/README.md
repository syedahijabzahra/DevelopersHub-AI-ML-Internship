# ❤️ Heart Disease Prediction

A machine learning project that predicts the presence of heart disease using the **Cleveland Heart Disease dataset** (UCI), comparing **Logistic Regression** and **Decision Tree** classifiers with full EDA and visualizations.

---

## 📌 Overview

This project builds and evaluates two classification models to predict whether a patient has heart disease based on 13 clinical features. It includes data preprocessing, exploratory data analysis, model training, evaluation metrics, ROC curves, and feature importance analysis.

---

## ✨ Features

- 📊 Full Exploratory Data Analysis (EDA) with visualizations
- 🔄 Data cleaning — missing value imputation with column medians
- ⚖️ Binary target encoding (0 = No Disease, 1 = Disease)
- 🤖 Two models: Logistic Regression & Decision Tree Classifier
- 📈 Evaluation with Accuracy, ROC-AUC, Confusion Matrix, Classification Report
- 🔍 Feature importance & coefficient visualization
- 📉 ROC Curve comparison between models

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` / `seaborn` | Data visualization |
| `scikit-learn` | ML models, preprocessing, metrics |
| `kagglehub` | (Optional) Kaggle dataset download |

---

## 📂 Dataset

**Source:** [UCI Cleveland Heart Disease Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data)

| Feature | Description |
|---------|-------------|
| `age` | Age in years |
| `sex` | Sex (1 = male, 0 = female) |
| `cp` | Chest pain type (0–3) |
| `trestbps` | Resting blood pressure |
| `chol` | Serum cholesterol (mg/dl) |
| `fbs` | Fasting blood sugar > 120 mg/dl |
| `restecg` | Resting ECG results |
| `thalach` | Maximum heart rate achieved |
| `exang` | Exercise-induced angina |
| `oldpeak` | ST depression |
| `slope` | Slope of peak exercise ST segment |
| `ca` | Number of major vessels (0–3) |
| `thal` | Thalassemia type |
| `target` | **0 = No Disease, 1 = Disease** |

---

## 🚀 Getting Started

### 1. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kagglehub -q
```

### 2. Run the Notebook

Open `Heart_Disease_Prediction.ipynb` in Jupyter or Google Colab and run all cells sequentially.

---

## 📊 Results

| Model | Accuracy | ROC-AUC |
|-------|----------|---------|
| Logistic Regression | ~85% | ~0.92 |
| Decision Tree | ~78% | ~0.84 |

> *Results may vary slightly due to random state and data splits.*

---

## 📈 Visualizations Generated

- Target class distribution (bar + pie chart)
- Feature correlation heatmap
- Age & Cholesterol distribution by target
- Categorical features vs target
- Confusion matrices (both models)
- ROC curve comparison
- Feature coefficients (LR) & feature importances (DT)

---

## 📁 Project Structure

```
Heart_Disease_Prediction/
│
├── Heart_Disease_Prediction.ipynb   # Main notebook
├── target_distribution.png
├── correlation_heatmap.png
├── age_chol_distribution.png
├── categorical_vs_target.png
├── confusion_matrices.png
├── roc_curves.png
├── feature_importance.png
└── README.md
```

---

## 🙋 Author

Built as part of an AI/ML internship project at **DevelopersHub Coorporation**.
