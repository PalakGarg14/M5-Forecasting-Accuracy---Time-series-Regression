# M5-Forecasting-Accuracy---Walmart

**Introduction**
This project aims to build accurate forecasting models for the M5 forecasting accuracy competition hosted by the Walmart Labs. The objective of the competition is to predict the daily sales for 28 different products across 10 stores, using historical sales data and external variables such as holidays and promotions.

**Data**
The dataset for this project includes historical sales data for 3049 products across 10 stores, as well as external variables such as calendar events and promotions. The data files can be accessed using Kaggle website for M5 Forecasting competition.

**Methodology**
We tried a variety of forecasting models for this project, such as L1 regression, decision trees, Light GBM. We also experimented with different input features, such as lagged sales data, rolling means and expanding mean window. For now the model has been evaluated on mean squared error (MSE) metric and R2 value. 

**Results**
Our best performing model was an Light GBM model that used a combination of lagged sales and rolling means sales data as input features. This model achieved an MSE of 3.05 on the training set and R2 value of 77%. 

                     Feature INFO                              |                  Model                   |  RMSE |  R2  |
+--------------------------------------------------------------+------------------------------------------+-------+------+
|                  A. Adding Simple Features                   |                                          |       |      |
|                             A.1                              | Linear regression with L1 regularization | 13.05 | 0.02 |
|                             A.2                              |              Decision Tree               |  8.77 | 0.34 |
|                             A.3                              |              LGBM Regressor              | 11.93 | 0.10 |
|                                                              |                                          |       |      |
|                    B. Adding Day Features                    |                                          |       |      |
|                             B.1                              | Linear regression with L1 regularization | 13.05 | 0.02 |
|                             B.2                              |              Decision Tree               |  8.68 | 0.35 |
|                             B.3                              |              LGBM Regressor              | 11.91 | 0.10 |
|                                                              |                                          |       |      |
| C. Adding lags, rolling window and expanding window Features |                                          |       |      |
|                             C.1                              | Linear regression with L1 regularization |  3.33 | 0.75 |
|                             C.2                              |              Decision Tree               |  7.64 | 0.42 |
|                             C.3                              |              LGBM Regressor              |  3.05 | 0.77 |



**Next Steps**:
The model is yet to be made as per the output required for the competition. Its a work in progress. Additionally, i will be focussing on tuning the hyperparameters for each model using a combination of grid search and manual tuning, and evaluated the performance of each model using the mean squared error (MSE) metric.

