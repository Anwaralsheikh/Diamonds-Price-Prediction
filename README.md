# 💎 Diamonds Price Prediction

A machine learning project that predicts the **price of diamonds** based on their physical and categorical attributes (such as carat, cut, color, and clarity).  
This project demonstrates the complete data science pipeline — from **data cleaning and feature engineering** to **model training, evaluation, and prediction**.

---

## 🧠 Project Overview
Diamonds vary widely in price depending on their characteristics.  
The goal of this project is to **build a regression model** that accurately predicts a diamond’s price given its features.

---

## 📊 Dataset
- **Source:** [Kaggle - Diamonds Dataset](https://www.kaggle.com/datasets/shivam2503/diamonds)
- **Size:** ~54,000 records
- **Features:**
  - **Carat:** Weight of the diamond.
  - **Cut:** Quality of the cut (Fair, Good, Very Good, Premium, Ideal).
  - **Color:** Diamond color, from D (best) to J (worst).
  - **Clarity:** Measurement of how clear the diamond is (IF, VVS1, VVS2, VS1, VS2, SI1, SI2, I1).
  - **Depth, Table:** Proportions of the diamond.
  - **x, y, z:** Physical dimensions.
  - **Price:** Target variable (USD).

---

## ⚙️ Project Workflow

1. **Data Loading and Cleaning**
   - Handle missing values (if any)
   - Remove outliers (e.g., extreme carat/price values)
   - Check for data consistency

2. **Exploratory Data Analysis (EDA)**
   - Distribution of prices and features
   - Correlation heatmap
   - Visualizations using Seaborn & Matplotlib

3. **Feature Engineering**
   - Encoding categorical features (Cut, Color, Clarity)
   - Feature scaling (StandardScaler / MinMaxScaler)
   - Creating new features such as *price per carat*

4. **Model Training**
   - Models tested:
     - Linear Regression
     - Random Forest Regressor
     - XGBoost Regressor
   - Hyperparameter tuning using GridSearchCV

5. **Model Evaluation**
   - Evaluation metrics:
     - Mean Absolute Error (MAE)
     - Root Mean Squared Error (RMSE)
     - R² Score
   - Comparison of models and selection of best performer

6. **Model Saving & Prediction**
   - Save the best model using `joblib`
   - Demonstrate prediction for new diamond input

---

## 📈 Results
| Model | MAE | RMSE | R² |
|--------|-----|------|----|
| Linear Regression | — | — | — |
| Random Forest | — | — | — |
| XGBoost | — | — | — |

👉 *(Fill in with your actual results once you run the models)*

Key insights:
- **Carat weight** is the most significant predictor of price.
- **Cut and Clarity** also affect the price, but to a lesser extent.
- Ensemble models (e.g., Random Forest, XGBoost) outperform simple linear models.

---

## 🧩 Requirements

To install required libraries:

```bash
pip install -r requirements.txt
