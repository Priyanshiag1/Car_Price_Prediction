**🚗 Car Price Predictor**

A machine learning web application that predicts the price of used cars based on features like brand, model, year, kilometers driven, and fuel type.  
The app is built with Flask for the web interface and uses a Linear Regression model trained on real-world car data.
## ✨ Features
- Predicts used car prices based on:
  - Car name/model
  - Company/brand
  - Year of manufacture
  - Kilometers driven
  - Fuel type
- User-friendly web interface (Flask)
- Data preprocessing and feature engineering
- One-hot encoding for categorical features
- Linear Regression model for prediction

## 🧠 Model Pipeline

### 🔹 Preprocessing:
- Cleaned and converted data types
- Handled missing values
- One-hot encoded categorical columns: `name`, `company`, `fuel_type`

### 🔹 Model:
- Used `LinearRegression` from scikit-learn
- Pipeline includes `ColumnTransformer` for encoding + regression model

### 🔹 Features Used:
- **Categorical:** name, company, fuel_type (OneHotEncoded)
- **Numerical:** year, kms_driven (passed through)

## 🌐 Web App (Flask)

- Simple web form to input car details
- Displays predicted price instantly
- Model is loaded from a `.pkl` file

### Usage
Open the web app in your browser.
Enter car details (brand, model, year, kms driven, fuel type).
Click Predict.
The predicted price will be displayed.
