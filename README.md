# 🍔 Food Delivery Time Prediction

## 📌 Project Description

This project focuses on predicting the delivery time of food orders based on various features such as restaurant location, customer location, order type, weather conditions, and more. The goal is to build a machine learning model that helps delivery services estimate accurate delivery times.

## 📊 Dataset

- [x] Source: [Kaggle Food Delivery Dataset](https://www.kaggle.com/datasets/gauravmalik26/food-delivery-dataset/data)
- [x] Features: Weather conditions, vehicle conditions, delivery person age, etc.
- [x] Target: Time taken to deliver the food (in minutes)

## 🛠️ Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn / XGBoost
- Matplotlib / Seaborn (for EDA)

## 🚀 Steps 
1. Data preprocessing
   a. Assigning appropriate data types to each column
   b. Handling missing values. For numerical variables, replaced with median or random values based on the distribution. For categorical variables, fill in with modes.
2. Feature Engineering
   a. Calculate the distance between restaurant and delivery placed location
   b. Creating other non-datetime variables to capture the information from the time order variable
   c. Correlation analysis to evaluate the correlation between the dependent variables and target variable. For numerical variable, use the Pearson Correlation while for          categorical variables used one-way ANOVA. Eliminating unnecessary variables with no significant correlations
3. Model Building with XGBoost, built a regression model using XGBoost using Cross Validation to search for the best combination of parameters possible resulting in the highest R2 possible.
