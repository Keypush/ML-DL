# Retail Project

Dataset Details: 
Attached

Training Data Description: Historic sales at Store-Day level for about two years for a retail giant, for more than 1000 stores. Also, other sale influencers like, whether on a particular day the store was fully open or closed for renovation, holiday and special event details, are also provided. 



DESCRIPTION

Demand Forecast is one of the key tasks in Supply Chain and Retail Domain in general. It is key in effective operation and optimization of retail supply chain. Effectively solving this problem requires knowledge about a wide range of tricks in Data Sciences and good understanding of ensemble techniques. 
You are required to predict sales for each Store-Day level for one month. All the features will be provided and actual sales that happened during that month will also be provided for model evaluation. 

Steps followed:

### Exploratory Data Analysis (EDA) and Linear Regression:
1. Transformed the variables by One-Hot Encoding 
2. Performed an EDA (Exploratory Data Analysis) to see the impact of variables over Sales.
3. Linear Regression to predict the forecast and evaluate different accuracy matrices like RMSE (Root Mean Squared Error) and MAE(Mean Absolute Error) and determine which metric makes more sense.
         a) Trained a single model for all stores, using storeId as a feature.
         b) Trained separate model for each store.
         c) Used Regularized Regression.

### Other Regression Techniques:
1. When store is closed, sales = 0, using this insight retrained the model.
2. Used Non-Linear Regressors, XGRegressors.
       a) Trained a single model for all stores, where storeId can be a feature.
       b) Trained separate models for each store.
       c) Used GridSearchCV for Tree’s Hyperparameter Tuning, Cross-validate to find best parameters. 
3. Trained a Time-series model on the data taking time as the only feature. This will be a store-level training. Identified yearly trends and seasonal months and used Seasonal ARIMA model.
 
### Implementing Neural Networks:
1. Trained a LSTM on the same set of features and compared the result with traditional time-series model.
2. Cluster stores using sales and customer visits as features. Found optimal clusters using Elbow-Method
3. Trained separate model for each clusters.


Trained all the features using the ANN model.s


