# 🌾 Crop Yield Prediction Using Machine Learning

This project explores how machine learning models can be used to predict crop yield (hg/ha) and classify performance levels (High vs Low) using country, crop, and time-based features.

## 📌 Problem Statement
Predict agricultural yield and identify low-performing regions or crop types using historical data. This helps governments, farmers, and agri-tech companies make informed decisions.

## 📊 Dataset
- Source: Kaggle (Crop Yield Prediction Dataset)
- Target Variable (Regression): `hg/ha_yield`
- Target Variable (Classification): `High_Yield` (binary from median threshold)
- Engineered features:
  - `Avg_Yield_by_Item`, `Avg_Yield_by_Area`
  - `Item_Area_Yield_Ratio`, `Is_Top_Item`, `Decade`

## 🧠 Models Used
### Regression
- XGBoost Regressor
- LightGBM Regressor
- CatBoost Regressor

### Classification
- XGBoost Classifier
- LightGBM Classifier
- CatBoost Classifier

## 📈 Evaluation Metrics
| Model     | Type          | RMSE / Accuracy | R² / F1 Score |
|-----------|---------------|------------------|----------------|
| XGBoost   | Regression     | ...              | ...            |
| LightGBM  | Regression     | ...              | ...            |
| CatBoost  | Regression     | ...              | ...            |
| XGBoost   | Classification | ...              | ...            |
| LightGBM  | Classification | ...              | ...            |
| CatBoost  | Classification | ...              | ...            |

_(Replace `...` with actual values from your summary CSV)_

## 📌 Key Insights
- Yield is highly influenced by **crop type** and **country**, as shown by feature importance.
- Time (decade) has minor influence, showing limited temporal trend.
- Classification helped flag high-risk crop-region combinations.

## 📂 Project Structure
- `notebooks/` – code files
- `data/` – input dataset
- `results/` – output CSV, plots
- `README.md` – this file

## 🛠️ Dependencies
```bash
pip install xgboost lightgbm catboost scikit-learn pandas seaborn matplotlib
```
[README.md](https://github.com/user-attachments/files/19461055/README.md)
op yield using ML with XGBoost, LightGBM, and CatBoost – includes regression and classification with engineered features
