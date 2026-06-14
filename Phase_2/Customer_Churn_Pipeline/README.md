# End-to-End ML Pipeline for Customer Churn Prediction

## 📌 Objective
Build a reusable, production-ready machine learning pipeline using Scikit-learn's Pipeline API to predict customer churn for a telecom company.

## 🛠 Methodology / Approach
- Loaded and cleaned the Telco Customer Churn dataset
- Built a preprocessing pipeline using ColumnTransformer (StandardScaler for numeric features, OneHotEncoder for categorical features)
- Trained two models within full pipelines: Logistic Regression and Random Forest
- Tuned hyperparameters using GridSearchCV with 5-fold cross-validation
- Evaluated models using Accuracy, F1 Score and Confusion Matrix
- Exported the best performing pipeline using joblib for production reusability

## 🛠 Technologies Used
- Python
- Scikit-learn (Pipeline, ColumnTransformer, GridSearchCV)
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Joblib

## 📊 Dataset
Telco Customer Churn Dataset
- Customer demographic, account and service usage data
- Binary target: Churn (Yes/No)

## 📈 Key Results
- Compared Logistic Regression and Random Forest pipelines with hyperparameter tuning
- Best model selected based on F1 Score
- Full preprocessing + model pipeline exported as a single reusable .joblib file

## 🚀 How to Run
1. Clone the repository
2. Install requirements: pip install scikit-learn pandas numpy matplotlib seaborn joblib
3. Run: customer_churn_pipeline.ipynb

## 👩‍💻 Author
Syeda Hijab Zahra
BS Software Engineering — UMT
AI/ML Engineering Intern — DevelopersHub Corporation
