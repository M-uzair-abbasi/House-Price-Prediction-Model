# House-Price-Prediction-Model
ML model for predicting house prices using XGBoost, feature engineering, and pipelines
# 🏠 House Price Prediction - Machine Learning Pipeline

This repository contains my solution to the Kaggle House Prices: Advanced Regression Techniques competition.

The project is built as a complete machine learning pipeline including data preprocessing, feature engineering, model training, and submission generation.

## 💡 Key Features

- **Missing Value Imputation**:  
  - Numerical columns imputed using median values.  
  - Categorical columns imputed using the most frequent values.

- **Feature Engineering**:  
  - Created new features like `TotalSF`, `TotalBathrooms`, and `HasPool`.

- **Encoding & Scaling**:  
  - One-hot encoding applied with `drop_first=True` to avoid multicollinearity.  
  - Features scaled using `StandardScaler`.

- **Model Used**:  
  - `Lasso Regression` with log-transformed target variable (`log1p`) for better performance.  
  - Achieved CV RMSE of approximately 0.13.

- **Submission**:  
  - Predictions inverse-transformed and saved to `submission.csv`.

## 📁 Files

- `house_pipeline.ipynb`: The main notebook containing all code for preprocessing, training, and submission.
- `submission.csv`: Final submission file for Kaggle leaderboard.

## 🔮 Possible Improvements

- Experiment with other models like `XGBoost`, `LightGBM`, or stacking.
- Perform hyperparameter tuning using `GridSearchCV` or `Optuna`.
- Add polynomial features or interaction terms for non-linear relationships.

## 📦 How to Use

1. Clone this repository.
2. Run `house_pipeline.ipynb` in a Jupyter environment.
3. Submit the generated `submission.csv` to Kaggle.

---

🎯 **Goal**: Improve ML skills by solving real-world regression problems using clean, interpretable pipelines.
