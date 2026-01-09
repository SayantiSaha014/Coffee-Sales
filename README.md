<h1 align="center"> ☕ Coffee Sales ☕ </h1>
  <div align="center">
</div>

<div align="center">
  <img src="Coffee Logo.png" width='170'>
</div>


# 📜 Introduction

This dataset contains detailed records of coffee sales from a vending machine. It is intended for the analysis of purchasing patterns, sales trends, and customer
preferences related to coffee products.

# 🗂 Dataset Overview 

● Date - Purchase date 

● DateTime - Date with transaction time 

● Coffee Name - Different types of coffee available 

● Cash type - Payment done by cash or card 

● Card - Card number 

● Money - Price per coffee ordered

# 🛠 Technology Stack
🐍 Python

# 📚 Python Libraries
- Pandas - Data manipulation
- NumPy - Statistical analysis
- Matplotlib & Seaborn - Data visualization
- scikit-learn - Machine Learning Library

# ⏲ Time-Series Analysis 

1) Daily Sales Aggregation
   a) Aggregated sales at a daily level
   b) Ensured continuous date index using asfreq(D)

   This step is crucial for accurate forecasting.

2) Product-Wise Time Series a) Created a pivot table:
                                                 i) Rows → Date
                                                 ii) Columns → Coffee Name
                                                 iii) Values → Daily sales amount

   b) Selected Top N products for modeling

# Forecasting & Predictive Modeling
1) Modeling Goal To predict: ● Future daily sales ● The coffee products will sell the most over time ● Expected revenue growth
   
2) Models Implemented Models that are implemented in this project for further analysis:
   
   ❖ SARIMAX (Statistical Model)

     ● Captures:
           ○ Trend
           ○ Seasonality
           ○ Autocorrelation

     ● Suitable for stable time-series patterns
   
   ❖ XGBoost Regressor (Machine Learning Model)

     ● Used expanding window time-series validation
   
3) Model Evaluation Metrics

   ● RMSE (Root Mean Squared Error)

   ● MAE (Mean Absolute Error)
  
   Lower error values indicate better predictive accuracy.

# 📑 Conclusion 

*This successfully gives a complete data analytics and forecasting pipeline on real-world coffee sales data. It combines EDA, customer analysis, and advanced time-series forecasting to provide actionable insights that can directly drive improvement in sales strategy, inventory control, and revenue planning. It combines the use of machine learning through XGBoost, using statistical models such as SARIMAX to provide high accuracy with interpretability for practical and scalable business deployment.*
