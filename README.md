#  Bengaluru House Price Prediction  
**Capstone Project – TECH-CRUSH 2024**  
By Esther D. S.

---

##  Overview  
This capstone project focuses on predicting house prices in Bengaluru, India using machine learning models. The dataset includes property features such as location, square footage, number of bathrooms, and more. The objective is to clean and prepare the data, explore it visually, and train predictive models to estimate housing prices accurately.

---

## Dataset Description  
- **Source**: Kaggle – Bengaluru House Data  
- **Target Variable**: `price` (in lakhs)  
- **Key Features**:  
  - `location`, `total_sqft`, `size`, `bath`, `balcony`, `area_type`

---

##  Data Cleaning & Wrangling  
- Converted non-numeric `total_sqft` values (ranges and text) into numerical format  
- Extracted number of bedrooms (`BHK`) from the `size` column  
- Removed extreme outliers in price per sqft  
- Handled missing values in `bath`, `balcony`, and other columns  
- Consolidated rare locations under `other` category  

---

## Exploratory Data Analysis (EDA)  
- Used visualizations to understand relationships between price, BHK, and location  
- Identified inconsistent pricing trends based on size and amenities  
- Generated correlation heatmaps and scatter plots for price vs sqft  

---

## Feature Engineering  
- Created new column `price_per_sqft`  
- One-hot encoded categorical features like `location` and `area_type`  
- Normalized numerical features for better model convergence

---

## Model Building  
- **Algorithms Tested**:  
  - Linear Regression  
  - Lasso Regression  
  - Decision Tree Regressor  
  - Random Forest Regressor  

- **Evaluation Metrics**:  
  - R² Score  
  - Mean Absolute Error (MAE)  
  - Root Mean Squared Error (RMSE)  

- **Best Model**: Random Forest with highest R² score on validation set

---

## Key Insights  
- Higher square footage doesn't always mean higher price per sqft  
- Location plays the most critical role in determining price  
- Properties with more than 4 BHK showed inconsistencies, likely due to data sparsity  

---

## Repository Contents  
- `CAPSTONE PROJECT TECH-CRUSH 2024 ESTHER D_S.ipynb` – Jupyter notebook with full project  
- `cleaned2_bengaluru_house_prices.csv` – Cleaned dataset  
- bengaluru_housing_encoded - Categorical data encoded 
- `README.md` – Project summary  

---

##  Author  
**Esther D. S.**  
[GitHub](https://github.com/OziomaEsther) | [LinkedIn](www.linkedin.com/in/francis-esther-ozioma-611ba6230)
