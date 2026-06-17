# Multimodal ML - Housing Price Prediction Using Images + Tabular Data

## 📌 Objective
Predict housing prices by combining structured tabular data with house image features using a multimodal deep learning approach.

## 🛠 Methodology / Approach
- Generated tabular housing features (square footage, bedrooms, bathrooms, age, garage)
- Generated corresponding house images encoding a visual "quality" signal correlated with housing features
- Built a dual-branch neural network: a CNN branch for image feature extraction and a dense network branch for tabular features
- Fused both feature representations via concatenation before final regression output
- Trained the combined model end-to-end for 30 epochs
- Evaluated performance using MAE, RMSE and R² Score

## 🛠 Technologies Used
- Python
- TensorFlow/Keras (Functional API, CNN, Dense layers)
- Scikit-learn (StandardScaler, evaluation metrics)
- Pandas
- NumPy
- Matplotlib

## 📊 Dataset
Synthetic housing dataset combining:
- Tabular features: square footage, bedrooms, bathrooms, age, garage spaces
- Corresponding generated house images encoding visual quality signals correlated with price

## 📈 Key Results
- MAE: $63,425.25
- RMSE: $76,443.63
- R² Score: 0.6871
- Demonstrated successful feature fusion between image and tabular modalities, with training and validation loss converging smoothly

## 🚀 How to Run
1. Clone the repository
2. Install requirements: pip install tensorflow scikit-learn pandas numpy matplotlib seaborn
3. Run: multimodal_housing_price.ipynb

## 👩‍💻 Author
Syeda Hijab Zahra
BS Software Engineering — UMT
AI/ML Engineering Intern — DevelopersHub Corporation
