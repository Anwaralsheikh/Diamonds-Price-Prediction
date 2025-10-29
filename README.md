# 💎 Diamonds Price Prediction

A machine learning project that predicts the **price of diamonds** based on their physical and categorical attributes (such as carat, cut, color, and clarity).  
This project demonstrates the complete data science pipeline — from **data cleaning and feature engineering** to **model training, evaluation, and prediction**.

---

##  Project Overview
Diamonds vary widely in price depending on their characteristics.  
The goal of this project is to **build a regression model** that accurately predicts a diamond’s price given its features.

---

##  Dataset
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

##  Project Workflow

1. **Data Loading and Cleaning**
   - Handle missing values (if any)
   - Remove outliers 
   - Check for data consistency

2. **Exploratory Data Analysis (EDA)**
   - Distribution of prices and features
   - Correlation heatmap
   - Visualizations using Seaborn & Matplotlib

3. **Feature Engineering**
   - Encoding categorical features (Cut, Color, Clarity)
   - Feature scaling (StandardScaler / MinMaxScaler)
   - Creating new features such as volume = x * y * z

4. **Model Training**
   - Models tested:
     - Linear Regression
     - Random Forest Regressor
     - XGBoost Regressor
     - Ridge Regression
     - Lasso Regression
     - Gradient Boosting
     - Decision Tree
     - Support Vector Regression (SVR)

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
| XGBoost | 134544.187500 | 366.802655 |0.980272 |
| Random Forest | 139550.757377 | 373.564931 | 0.979537 |
| Decision Tree | 232311.169679| 481.986690 | 0.965936|
| Gradient Boosting | 305716.417029 | 552.916284| 0.955172|
| SVR | 336387.855839 | 579.989531 | 0.950675 |
| Linear Regression | 513955.377862 | 716.906813 | 0.924638 |
| Ridge Regression | 514273.702109 | 717.128790| 0.924591|
| Lasso Regression | 514830.097745 | 717.516618| 0.924509|



Key insights:
- **Carat weight** is the most significant predictor of price.
- **Cut and Clarity** also affect the price, but to a lesser extent.
- Ensemble models (e.g., Random Forest, XGBoost) outperform simple linear models.

---

##  Requirements

To install required libraries:

```bash
pip install -r requirements.txt
