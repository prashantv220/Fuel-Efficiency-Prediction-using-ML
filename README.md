# Car Price Prediction using Machine Learning

## 📖 Overview
This project aims to predict **car prices** based on different attributes such as mileage, year, fuel type, transmission, and engine specifications.  
By applying multiple regression techniques, we can evaluate how well each method captures the relationship between car features and their market value.  

Car price prediction is useful for:
- Buyers who want a fair estimate before purchase  
- Sellers/dealers to set competitive prices  
- Automobile businesses to understand market trends  

---

## 📂 Dataset
The dataset used includes features such as:
- **Car brand and model**
- **Year of manufacture**
- **Fuel type (Petrol, Diesel, etc.)**
- **Transmission (Manual/Automatic)**
- **Mileage and Engine capacity**
- **Selling price** 

The data was cleaned to remove duplicates, handle missing values, and encode categorical features.

---

## 🔍 Approach

### 1. Data Preprocessing
- Removed inconsistencies and outliers (e.g., unrealistic mileage or prices)  
- Converted categorical variables to numeric form  
- Standardized/normalized numerical features for better model performance  
- Split data into **training (80%)** and **testing (20%)** sets  

### 2. Exploratory Data Analysis (EDA)
- Checked feature distributions (e.g., car age vs. price)  
- Visualized relationships using scatter plots, histograms, and heatmaps  
- Observed strong correlations between features like car age, fuel type, and price  

### 3. Model Building
We tested three different regression approaches:
1. **Linear Regression**  
   - Simple model assuming a straight-line relationship  
   - Useful as a baseline  
2. **Lasso Regression**  
   - Adds regularization to prevent overfitting  
   - Automatically reduces less useful features  
3. **XGBoost Regressor**  
   - Advanced ensemble technique  
   - Captures complex non-linear interactions  
   - Outperformed both linear and lasso in terms of accuracy  

### 4. Model Evaluation
The models were evaluated using:
- **R² Score** → how much variance in price is explained by the model  
- **Mean Absolute Error (MAE)** → average prediction error  
- **Root Mean Squared Error (RMSE)** → penalizes larger errors more heavily  

---

## 📊 Results

- **Linear Regression:** Provided a reasonable baseline but struggled with non-linear data  
- **Lasso Regression:** Improved feature selection and reduced overfitting  
- **XGBoost:** Delivered the best performance with the highest R² score and lowest errors  

Overall, **XGBoost Regressor proved to be the most reliable model** for predicting car prices.  

---

## 🚀 Usage
To explore the models:
- Open the Jupyter Notebooks:
  - `Car_Price_Prediction_using_Machine_Learning.ipynb`
  - `Using_XGboost_Regressor.ipynb`
- Run the cells to see preprocessing, model training, and evaluation  

Dependencies:  
`numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`  

---

## 🌟 Future Enhancements
- Hyperparameter tuning for XGBoost to push performance further  
- Add more advanced models (Random Forest, LightGBM, Neural Networks)  
- Incorporate more real-world features (car condition, demand, resale trends, region)   

---

## 📝 License
This project is licensed under the MIT License.
