## Car Price Prediction with Machine Learning
# Introduction
Car price prediction is a crucial aspect of the automotive industry, helping buyers, sellers, and manufacturers determine the fair value of a vehicle based on various attributes. In this project, we build a machine learning model to predict car prices using historical data.

# Dataset Overview
The dataset contains various features that influence car prices, such as:

+ Car Name – The brand/model of the car
+ Year – The year the car was manufactured
+ Selling Price – The price at which the car was sold (Target Variable)
+ Present Price – The current market value of the car
+ Kms Driven – The total distance the car has been driven
+ Fuel Type – Petrol/Diesel/CNG
+ Seller Type – Individual or Dealer
+ Transmission – Manual or Automatic
+ Owner – Number of previous owners

# Data Preprocessing
Before training the model, we performed the following preprocessing steps:

+ Checked for missing values and handled them appropriately
+ Converted categorical features (Fuel Type, Seller Type, Transmission) into numerical values using Label Encoding
+ Standardized numerical features for better model performance

# Machine Learning Model
We trained a Random Forest Regressor to predict car prices. The dataset was split into 80% training and 20% testing. Feature scaling was applied to ensure a consistent range for all features.

# Model Evaluation
The performance of the model was evaluated using the following metrics:

+ Mean Absolute Error (MAE) – Measures average error between actual and predicted prices
+ Mean Squared Error (MSE) – Penalizes larger errors more than smaller ones
+ Root Mean Squared Error (RMSE) – Square root of MSE for better interpretability
+ R-squared Score (R²) – Measures how well the model explains the variance in car prices.

# Visualization
The scatter plot "Actual vs Predicted Selling Prices" shows the relationship between the actual car prices and the prices predicted by the machine learning model. Here’s what it indicates:

+ Strong Positive Correlation: Most points align closely with a diagonal line (y = x), meaning the model is making good predictions.
+ Deviations from the Line: Some points deviate slightly, indicating minor prediction errors.
+ Outliers: A few points are further away, suggesting that the model might struggle with extreme values or rare cases.

![image alt](https://github.com/Engr-Usman-Ali/CodeAlpha_Task_Car_Prediction/blob/bcb7021e24fac57de6957cb568acd2a828e0ddac/car%20prediction.png)

Overall, this plot suggests that the model performs well, with reasonable accuracy in predicting car prices.

# Conclusion
This project successfully predicts car prices using machine learning. The Random Forest model performed well with a high R² score, indicating accurate predictions.
