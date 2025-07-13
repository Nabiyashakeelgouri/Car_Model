# Car_Price_Prdeiction_Model
This project focuses on building a simple Linear Regression model to predict the resale price of cars based on various features such as brand, engine size, fuel type, transmission, mileage, age, and condition.
# 🚗 Car Price Prediction Model

This project is a **Linear Regression model** built to predict the price of cars based on features such as brand, engine size, fuel type, transmission, mileage, and condition.

## 📁 Dataset

The dataset includes the following columns:
- `Car ID`
- `Brand`
- `Year`
- `Engine Size`
- `Fuel Type`
- `Transmission`
- `Mileage`
- `Condition`
- `Price`
- `Model`

🔧 We calculated a new column:
- `Car Age = 2025 - Year` (to get the vehicle's age)

Outliers in the `Price` column were removed to improve accuracy.

---

## 🧠 Objective

Build a simple, interpretable regression model using:
- One-hot encoding for categorical features
- Linear regression for continuous prediction
- Evaluation using R² Score and Mean Squared Error

---

## 🔍 Libraries Used

- `pandas` – Data handling
- `matplotlib` – Visualization
- `scikit-learn` – Model building, preprocessing, evaluation

---

## ⚙️ Model Pipeline

The machine learning pipeline includes:

1. **Preprocessing**
   - Categorical variables (`Brand`, `Fuel Type`, `Transmission`, `Condition`) are encoded using **OneHotEncoder**
   - Numeric columns are passed as-is (`passthrough`)

2. **Model**
   - A **Linear Regression** model is applied on the transformed data

---

## 📊 Evaluation Metrics

- **R² Score** – Indicates how well the model explains the variance in price
- **Mean Squared Error (MSE)** – Measures average squared error between actual and predicted prices

---

## 📈 Visualization

The output includes a **scatter plot** comparing actual vs predicted car prices to visualize model accuracy.

---

## ✅ How to Run

1. Install required libraries (if not already installed):
   ```bash
   pip install pandas matplotlib scikit-learn
