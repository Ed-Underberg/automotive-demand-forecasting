# Forecasting U.S. Vehicle Sales with Macroeconomic and Financial Data

> **A time series forecasting analysis comparing traditional regression, autoregressive (ARX), and machine learning models to predict U.S. vehicle demand (SAAR).**

---

## Executive Summary

Automotive manufacturers, suppliers, dealer groups, and market intelligence teams rely on accurate demand forecasts to support production planning, inventory management, pricing strategy, and capital investment decisions.

This project investigates how macroeconomic conditions and financial market indicators influence U.S. light vehicle sales (Seasonally Adjusted Annual Rate, **SAAR**) while evaluating multiple statistical and machine learning forecasting approaches.

Beginning with traditional regression analysis, the modeling framework progressively incorporates lagged variables, autoregressive time-series techniques, and machine learning models to improve predictive performance and better capture the dynamics of vehicle demand.

---

## Key Result

**The highest-performing model—an Autoregressive model with exogenous macroeconomic indicators (ARX)—achieved an out-of-sample R² greater than 0.66 on a held-out 20% test set, explaining approximately two-thirds of the variation in next month's U.S. vehicle sales.**

---

## Business Problem

Vehicle demand is influenced by a broad set of economic forces including:

- Consumer confidence
- Employment
- Inflation
- Interest rates
- Gasoline prices
- Financial market performance
- Market volatility

Understanding which factors are most influential—and how they interact over time—can improve forecasting accuracy and support more informed business decisions across the automotive value chain.

---

## Research Questions

This analysis addresses three primary questions:

### 1. Financial Markets

Which financial market indicators—including equity market performance, market volatility (VIX), and inflation—are most closely associated with changes in U.S. vehicle sales?

### 2. Macroeconomic Conditions

Which macroeconomic indicators—such as consumer sentiment, recession conditions, unemployment, and gasoline prices—provide meaningful insight into vehicle demand?

### 3. Forecasting

Can macroeconomic indicators, combined with autoregressive time-series modeling, improve one-month-ahead forecasts of U.S. vehicle sales?

---

## Data

**Observation Frequency**

Monthly

**Study Period**

April 2000 – January 2026

**Target Variable**

Seasonally Adjusted Annual Rate (SAAR) of U.S. Light Vehicle Sales

**Primary Sources**

- Federal Reserve Economic Data (FRED)
- Yahoo Finance

---

## Modeling Workflow

The project follows a structured analytical progression:

1. Exploratory Data Analysis
2. Multiple Linear Regression
3. Lagged Regression Analysis
4. Autoregressive Modeling with Exogenous Variables (ARX)
5. Random Forest Regression
6. K-Nearest Neighbors Regression
7. Model Comparison & Evaluation

---

## Technologies

- Python
- pandas
- NumPy
- statsmodels
- scikit-learn
- matplotlib

---

## Evaluation Metrics

Models were evaluated using a chronological 80/20 train-test split.

Performance metrics include:

- Out-of-Sample R²
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)

---

## Repository Structure

```text
automotive-demand-forecasting/

├── notebooks/
│   └── automotive-demand-forecasting-time-series.ipynb
│
├── data/
│   └── Auto Sales Data.csv
│
├── images/
│
└── README.md
```

---

## Potential Business Applications

- Automotive demand forecasting
- Production planning
- Inventory optimization
- Dealer network planning
- Pricing strategy
- Market intelligence
- Economic scenario planning

---

## Future Enhancements

Potential future improvements include:

- XGBoost and LightGBM models
- Rolling-origin cross-validation
- SHAP value analysis for model explainability
- Automated forecasting pipeline
- Interactive Tableau dashboard
- Scenario-based forecasting using projected macroeconomic conditions

---

## Author

**Ed Underberg**

Senior Marketing and Analytics Consultant

LinkedIn: https://www.linkedin.com/in/ed-underberg/
Email: edunderberg@gmail.com

---
