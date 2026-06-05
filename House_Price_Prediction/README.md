# 🏠 House Price Prediction

A regression project that predicts California house prices using the **California Housing Dataset** (scikit-learn), comparing **Linear Regression**, **Ridge Regression**, and **Gradient Boosting** with feature engineering and comprehensive visualizations.

---

## 📌 Overview

This project builds and evaluates three regression models to predict median house prices across California districts. It includes feature engineering, EDA, model training with scaling, performance comparison using MAE/RMSE/R², and visual analysis including predicted vs. actual plots and residual analysis.

---

## ✨ Features

- 📊 Exploratory Data Analysis with price distributions and scatter plots
- 🔧 Feature engineering — `rooms_per_person`, `bedrooms_per_room`, `population_density`
- ⚖️ StandardScaler for Linear and Ridge models
- 🤖 Three models: Linear Regression, Ridge Regression, Gradient Boosting
- 📈 Evaluation with MAE, RMSE, and R² score
- 📉 Predicted vs. Actual plots for all three models
- 🔍 Residual analysis and feature importance (GBR)

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` / `seaborn` | Data visualization |
| `scikit-learn` | Dataset, models, preprocessing, metrics |

---

## 📂 Dataset

**Source:** California Housing Dataset — `sklearn.datasets.fetch_california_housing`

| Feature | Description |
|---------|-------------|
| `MedInc` | Median income (in $10k) |
| `HouseAge` | Median house age |
| `AveRooms` | Average number of rooms |
| `AveBedrms` | Average bedrooms per household |
| `Population` | Block population |
| `AveOccup` | Average occupancy |
| `Latitude` | Latitude |
| `Longitude` | Longitude |
| `price` | **Target: Median house value (USD)** |

> Price is converted from 100k units to actual USD for readability.

---

## 🚀 Getting Started

### 1. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn -q
```

### 2. Run the Notebook

Open `House_Price_Prediction.ipynb` in Jupyter or Google Colab and run all cells.

> ⚠️ Gradient Boosting training takes approximately 1–2 minutes.

---

## 📊 Results

| Model | MAE | RMSE | R² |
|-------|-----|------|-----|
| Linear Regression | ~$50,000 | ~$74,000 | ~0.60 |
| Ridge Regression | ~$50,000 | ~$74,000 | ~0.60 |
| Gradient Boosting | ~$32,000 | ~$51,000 | ~0.84 |

> *Gradient Boosting significantly outperforms linear models on this dataset.*

---

## 📈 Visualizations Generated

- House price distribution (raw + log-transformed)
- Feature correlation heatmap
- Scatter plots: top features vs. price
- Model comparison bar chart (MAE, RMSE, R²)
- Predicted vs. Actual plots for all 3 models
- Residuals vs. Predicted & Residual distribution (GBR)
- Feature importance (Gradient Boosting)

---

## 📁 Project Structure

```
House_Price_Prediction/
│
├── House_Price_Prediction.ipynb   # Main notebook
├── price_distribution.png
├── correlation_heatmap.png
├── feature_vs_price.png
├── model_comparison.png
├── predicted_vs_actual.png
├── residuals.png
├── feature_importance.png
└── README.md
```

---

## 🙋 Author

Built as part of an AI/ML internship project at **DevelopersHub Coorporation*.
