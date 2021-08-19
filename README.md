# Capstone Project
# Prediction of the German Imbalance Energy Price

by Christian Dischke, Boris Geller, Jaouad El Yousfi, Matthias Schmidt

The project aims at predicting the imbalance energy
price (reBAP) for the German power transmission
nets. This price captures the costs of the net
balancing mechanism in time steps of 15 minutes. 

The imbalance energy price is mainly determined by unpredictable events. 
Therefore, its value at the time being is poorly related to its value at some former time 
and it cannot be predicted satisfactorily by an ordinary univariate time series model. 
For results on that approach, see the Jupyter notebook `KATS_time_series.ipynb` of Boris' repository 
https://github.com/Antadurunnu/Energy-imbalance-price-prediction.

For multivariate time series models using adapted neural networks, see the directory `4_Modelling` 
of Jaouad's repository https://github.com/Jaoaud/Capstone_Energy. 

Here, we follow a ML approach by predicting the imbalance energy price directly (regression) or intervals it belongs to (classification) from 
- dummified time variables, 
- live features publicly available with some delay,
- several forecasts.

The repository contains a python script for training and prediction and a jupyter notebook for data exploration.
While the model used here is a random forest, the script can be run with any regressor or classifier provided by sklearn 
and it can effortlessly be adapted to neural networks.
