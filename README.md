# 🚗 Car Price Prediction with Linear Regression

## 📘 Overview
This project builds a machine learning model to predict used car selling prices based on historical sales data. It includes data cleaning, exploratory analysis, feature engineering, and model training using Linear Regression.

## 📊 Dataset Info
- Source: `car data.csv`
- Records: 301 → 278 (after outlier removal)
- Features include:
  - Present_Price, Kms_Driven, Age (from Year)
  - Fuel_Type, Seller_Type, Transmission, Owner
- Target variable: `Selling_Price`

## 🔧 Preprocessing
- Removed irrelevant columns (e.g., Car_Name)
- Handled outliers using IQR
- Converted categorical variables using one-hot encoding
- Added polynomial features for better prediction

## 📈 Exploratory Analysis
- Average selling price: ₹4.66 lakhs  
- Key correlations:
  - Present_Price: **strong positive**
  - Age: **moderate negative**

## 🤖 Model Summary
- Model: **Linear Regression with Polynomial Features**
- R² Score: **0.903**
- Mean Squared Error: **1.054**
- Strong predictors: Present_Price, Age, Fuel_Type, Seller_Type

## 💡 Prediction Example
Given a car with:
- ₹5.59L present price, 27,000 km driven, 5 years old  
→ **Predicted Selling Price**: ₹3.83 lakhs

## ▶️ How to Use
1. Install dependencies: `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`
2. Load the dataset and preprocess it
3. Train the model and make predictions using:

