# M5-Forecasting-Accuracy---Walmart

**Introduction**
This project aims to build accurate forecasting models for the M5 forecasting accuracy competition hosted by the Walmart Labs. The objective of the competition is to predict the daily sales for 28 different products across 10 stores, using historical sales data and external variables such as holidays and promotions.

**Data**
The dataset for this project includes historical sales data for 3049 products across 10 stores, as well as external variables such as calendar events and promotions. The data files can be accessed using Kaggle website for M5 Forecasting competition.

**Methodology**
We tried a variety of forecasting models for this project, such as L1 regression, decision trees, Light GBM. We also experimented with different input features, such as lagged sales data, rolling means and expanding mean window. For now the model has been evaluated on mean squared error (MSE) metric and R2 value. 

**Results**
Our best performing model was an Light GBM model that used a combination of lagged sales and rolling means sales data as input features. This model achieved an MSE of 3.05 on the training set and R2 value of 77%. 

**Next Steps**:
The model is yet to be made as per the output required for the competition. Its a work in progress. Additionally, i will be focussing on tuning the hyperparameters for each model using a combination of grid search and manual tuning, and evaluated the performance of each model using the mean squared error (MSE) metric.

