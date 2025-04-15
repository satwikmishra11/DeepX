# DeepX
# Retail Demand Forecasting for Kirana Stores 

A comprehensive solution for predicting product demand in small retail (Kirana) stores.

##  Features
- **Hybrid Forecasting**: SARIMA + XGBoost ensemble model
- **Explainable AI**: SHAP values for feature importance
- **End-to-End Pipeline**: From EDA to production-ready forecasts

##  Repository Structure
.
├── data/
│ ├── kiranaRO_train.csv # Training transactions
│ ├── kiranaRO_test.csv # Future demand data
│ ├── product_catalog.csv # Item metadata
│ └── ... # Other supporting files
├── notebooks/
│ ├── EDA.ipynb # Exploratory analysis
│ └── Forecasting.ipynb # Model training/predictions
└── README.md # You are here

## Installation
```bash
pip install pandas numpy matplotlib seaborn statsmodels xgboost shap jupyter
```
 Usage:-
Generate Synthetic Data (if needed):

```bash
python generate_data.py
```
Run EDA:

```bash
jupyter notebook notebooks/EDA.ipynb
```
Run Forecasting:

```bash
jupyter notebook notebooks/Forecasting.ipynb
```
Key Results:-
Metric	SARIMA	XGBoost	Ensemble
MAE	23.4	19.8	17.2
