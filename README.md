# Daily Accident Volume Forecasting by Region

This project uses machine learning models to forecast daily traffic accident counts across UK regions. It was developed as part of the "Machine Learning for Business Analytics" coursework.

## 🚗 Problem Statement

A UK-based road assistance company needs accurate daily accident forecasts to improve emergency resource allocation. The aim is to predict the number of daily accidents per region using temporal, spatial, and environmental features.

## 📂 Dataset

Prepared from UK Department for Transport records and includes:
- Accident dates and locations
- Regional metadata (e.g., `region_name`)
- Weather and road surface conditions
- Aggregated accident counts per day per region

Files:
- `final_train_dataset.csv`
- `final_test_dataset.csv`

## 📊 Models

Models used:
- **Baseline**:
  - Seasonal Naïve
  - Linear Regression
- **Advanced**:
  - Random Forest Regressor (with hyperparameter tuning)
  - XGBoost Regressor

## 🧪 Evaluation Metrics

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score

## 🗺️ Spatial Analysis

Used GeoPandas and Folium to visualize regional prediction errors and accident clusters.

## 📈 Results

| Model             | MAE   | RMSE  | R²     |
|------------------|-------|-------|--------|
| Seasonal Naïve    | 1.88  | 3.86  | -2.33  |
| Linear Regression | 0.37  | 1.21  | 0.03   |
| Random Forest     | 0.34  | 1.25  | -0.04  |
| XGBoost           | 0.34  | 1.23  | 0.004  |

## 💡 Future Work

- Add traffic volume, holidays, or weather events as features
- Test LSTM or other deep learning models
- Regional-specific models to handle heterogeneity
