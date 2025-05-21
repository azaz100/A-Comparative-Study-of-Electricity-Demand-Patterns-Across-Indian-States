# A-Comparative-Study-of-Electricity-Demand-Patterns-Across-Indian-States

This repository contains the code, dataset, and results for a time series forecasting project that aims to model and compare electricity demand across various Indian states using two state-of-the-art methods: **XGBoost** and **Facebook Prophet**.

---

## 📌 Project Overview

Electricity demand forecasting is critical for ensuring grid stability and effective energy management in a country like India, which experiences diverse climatic and socio-economic conditions across states. This project builds a state-wise forecasting framework using:
- **XGBoost**: A powerful gradient-boosted decision tree model that excels at capturing nonlinear and complex relationships.
- **Facebook Prophet**: A time series forecasting model designed to decompose and interpret trends and seasonal patterns.

Both models are evaluated using metrics such as **R² Score**, **RMSE**, **MAE**, and **MAPE**, and are compared for performance across different Indian states.

---

## 📂 Project Structure

(root)

├── data/ # Cleaned and preprocessed dataset (filtered_2014_2024.csv)

├── results/ # Output files, plots, SHAP graphs, and visualizations

├── models/ # Trained models or prediction scripts (optional)

├── TSA_CODE.ipynb # Main Jupyter Notebook for training and comparison

├── README.md # This file

├── requirements.txt # Python dependencies

└── LICENSE # Optional open-source license



---

## 🛠️ How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/azaz100/A-Comparative-Study-of-Electricity-Demand-Patterns-Across-Indian-States.git
cd A-Comparative-Study-of-Electricity-Demand-Patterns-Across-Indian-States
```

### 2. Set Up the Environment

python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
pip install -r requirements.txt

### 3. Run the Notebook

Launch the Jupyter notebook to explore the data, run the models, and view visualizations:

jupyter notebook TSA_CODE.ipynb


📊 Features

a.> State-wise electricity demand forecasting

b.> Climate-aware modeling using UTCI (Universal Thermal Climate Index)

c.> XGBoost-based feature engineering and prediction

d.> Prophet-based trend and seasonality modeling

e.> Model performance evaluation using R², RMSE, MAE, MAPE

f.> SHAP-based model interpretation

g.> Visualizations for each state's actual vs. predicted demand

h.> Geographic heatmaps of model accuracy


🧪 Evaluation Metrics

| Metric   | Description                                   |
| -------- | --------------------------------------------- |
| R² Score | Variance explained by the model               |
| RMSE     | Emphasizes large errors                       |
| MAE      | Mean of absolute prediction errors            |
| MAPE     | Relative accuracy useful for comparing states |


📈 Sample Visualizations

Actual vs Predicted demand plots (for states like Andhra Pradesh and Odisha)

SHAP summary plots for XGBoost feature importance

R² Score maps for both XGBoost and Prophet models across India


🧠 Models Used

🔸 XGBoost
Gradient boosting algorithm for regression

Handles complex nonlinear relationships

Requires engineered features (day, month, etc.)


🔸 Facebook Prophet
Additive model for time series

Automatically models trend, seasonality, and holidays

Best suited for long-term trend interpretation


📋 Dataset
File: filtered_2014_2024.csv

Main Columns include:

a.> date

b.> state

c.> utci_mean: Universal Thermal Climate Index (target variable)

Additional weather and time-based features


