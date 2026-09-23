# ⚡ Energy Load Forecasting - Netherlands (ENTSO-e 2024)

![Python](https://img.shields.io/badge/Python-3.12-blue)
![XGBoost](https://img.shields.io/badge/XGBoost-2.0-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

A time series forecasting project analyzing and predicting hourly electricity load for the Netherlands using ENTSO-e Transparency Platform data.

## 📋 Project Overview

This project builds a baseline forecasting model for the Netherlands' hourly energy consumption to support grid management and capacity planning. Using calendar-based features and XGBoost, the model captures daily and seasonal demand patterns while identifying opportunities for improvement.

## 🎯 Key Results

| Metric | Value |
|--------|-------|
| **Test RMSE** | ~1,594 MW |
| **Train RMSE** | ~718 MW |
| **Error Rate** | ~12.2% of average load |
| **Dataset Size** | 8,784 hourly records |
| **Train/Test Split** | Before/After Oct 1, 2024 |

### Feature Importance
- **Hour** (~39%) - Strongest predictor
- **Day of Month** (~28%)
- **Day of Week** (~15%)
- **Day of Year** (~12%)
- **Month** (~5%)
- **Quarter** (0%)

## 📊 Visualizations

### Data Distribution & Patterns
![Weekly Pattern](images/week_pattern.png)
*Hourly load showing clear daily cycles*

### Feature Importance
![Feature Importance](images/feature_importance.png)
*XGBoost feature importance ranking*

### Predictions vs Actual
![Predictions](images/predictions_vs_actual.png)
*Model predictions vs actual load values*

## 🔧 Technical Stack

- **Python 3.12**
- **XGBoost** - Gradient boosting framework
- **Pandas** - Data manipulation
- **Scikit-learn** - Model evaluation
- **Matplotlib/Seaborn** - Visualization

## 📁 Project Structure
