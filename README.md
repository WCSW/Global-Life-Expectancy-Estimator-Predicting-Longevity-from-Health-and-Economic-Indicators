# Global-Life-Expectancy-Estimator-Predicting-Longevity-from-Health-and-Economic-Indicators
# Life Expectancy Estimator: Predicting Longevity from Global Indicators

## 🌍 Overview
This project predicts **life expectancy** using global health, demographic, and economic indicators. It demonstrates advanced regression modeling, data preprocessing, model evaluation, and explainability.

## 📁 Dataset
- **File:** `Life_Expectancy_Data.csv`
- **Records:** 2,938
- **Features:** Health metrics, GDP, immunizations, alcohol use, schooling, population, etc.
- **Target:** `Life expectancy` (float)

## ⚙️ Features
- Missing Value Imputation
- Categorical Encoding (e.g., `Status`)
- Feature Scaling
- Model Comparison: Linear Regression, Ridge, Random Forest, XGBoost
- Visualizations with Plotly
- SHAP for feature importance

## 📊 Results
Best model: **XGBoost Regressor**

| Model           | MAE   | MSE   | R²    |
|----------------|-------|-------|-------|
| XGBoost        | ~1.5  | ~4.5  | ~0.97 |
| Random Forest  | ~2.1  | ~6.3  | ~0.94 |

> 📈 SHAP indicates that `Schooling`, `Income composition`, and `HIV/AIDS` rate are top predictors of life expectancy.

## 🧠 Tech Stack
- Python (Pandas, Scikit-learn, XGBoost, SHAP)
- Plotly (for interactive plots)
- Jupyter Notebook

## 🧪 How to Run
```bash
pip install -r requirements.txt
jupyter notebook

