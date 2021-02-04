# Prediction-of-water-content-outcomes-in-gas-dehydration-systems-using-AI
An artificial neural network model will be created to predict the water content outcomes of natural gas dehydration systems. 


#Summary
This is an artificial neural network model used for predicting the water content outcomes of a natural gas dehydration system. The water content outcomes are either class 0 or class 1.

Class 0 represents data points that meet the sales gas pipeline quality water content specification of 7 lbs/MMscf and class 1 represents data points that do not meet the sales gas pipeline quality water content specification of 7 lbs/MMscf. 

#Data used
The data consists of four input features and one target output used in training and testing the artificial neural network model. The features are TEG recirculation rate (represented as TEG_recirc_rate), number of equilibrium stages (represented as no_of_equili_stages), temperature of the reboiler (represented as temp), and stripping gas flow rate (represented as stripping_rate). These three features, temperature of the reboiler, number of equilibrium stages, and stripping rate are ordinal categorical data while the last feature, TEG circulation rate is numerical continuous data. 
