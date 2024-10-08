# ✈️ Flight Fare Prediction Project

## 📝 Overview
This project focuses on predicting air ticket prices for domestic flights within India using machine learning techniques. The model is designed to analyze various factors that influence ticket pricing, such as airline, route, departure time, and more, enabling both airlines and passengers to make data-driven decisions.

## 📂 Project Structure

1. **📖 Introduction**
   - The project addresses the challenge of dynamic air ticket pricing in the Indian aviation industry.
   - By analyzing historical data, the model aims to accurately predict ticket prices and provide insights for better pricing strategies.

2. **📊 Data Details**
   - The dataset consists of 10,683 rows and 11 columns, representing key flight details.
   - Features include `Airline`, `Date_of_Journey`, `Source`, `Destination`, `Route`, `Dep_Time`, `Arrival_Time`, `Duration`, `Total_Stops`, `Additional_Info`, and `Price` (target variable).

3. **🔍 Exploratory Data Analysis**
   - Null values and outliers were identified and handled appropriately.
   - The analysis revealed trends such as the impact of the number of stops on ticket prices and the fluctuation of prices based on the airline.

4. **⚙️ Feature Engineering**
   - Nominal variables like `Airline`, `Source`, and `Destination` were one-hot encoded.
   - The `Route` feature was dropped due to its close relation to `Total_Stops`.
   - `Dep_Time` and `Arrival_Time` were broken down into hours and minutes.
   - The target variable `Price` is what the model aims to predict.

5. **🤖 Model Training**
   - Multiple regression models were tested, including `GradientBoostingRegressor`, `XGBRegressor`, `DecisionTreeRegressor`, and `SVR`.
   - Tuned `GradientBoostingRegressor` and `XGBRegressor` were identified as the top performers with R² scores of 0.867 and 0.861, respectively.

6. **✅ Conclusion**
   - The project recommends using the tuned `XGBRegressor` for optimal performance in predicting flight prices.
   - `GradientBoostingRegressor` is also suggested for its balance between accuracy and interpretability.
