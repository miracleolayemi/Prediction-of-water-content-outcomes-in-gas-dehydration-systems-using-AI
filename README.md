# Prediction-of-water-content-outcomes-in-gas-dehydration-systems-using-AI
An artificial neural network model will be created to predict the water content outcomes of natural gas dehydration systems. 


# Summary
This is an artificial neural network model used for predicting the water content outcomes of a natural gas dehydration system. The water content outcomes are either class 0 or class 1.

Class 0 represents data points that meet the sales gas pipeline quality water content specification of 7 lbs/MMscf and class 1 represents data points that do not meet the sales gas pipeline quality water content specification of 7 lbs/MMscf. 

# Data used
The source of the data is secondary data from the work of Hernandez-Valencia et al., (1992). 
The data consists of four input features and one target output used in training and testing the artificial neural network model. The features are TEG recirculation rate (represented as TEG_recirc_rate), number of equilibrium stages (represented as no_of_equili_stages), temperature of the reboiler (represented as temp), and stripping gas flow rate (represented as stripping_rate). 

# Exploratory Data analysis
A preliminary exploratory data analysis was done :i.e the use of visual plots and charts to have insight on the type of data, statistical significance of the data, and relationship between features in the data.  The insights from this analysis provide a well-rounded input when building the model. All statistics calculation was carried out with the Pandas library and all plots have been created with the Seaborn library in Python. 

# Model development
The ANN model was developed and fitted a three layer artificial neural network model with input features, reboiler temperature, number of equilibrium stages, triethylene glycol recirculation rate and stripping gas rate and output feature water content using back propagation method to minimize the error and Adam optimizer to optimize the weights. The hidden layer will contain seven nodes

# Model Evaluation
The model was evaluated and validated  for the model loss, accuracy, confusion matrix, precision score, recall score, and F1 score using independent validation dataset apart from the training data set.

# Evaluation with experimental literature data
Compare the Water content outcome predictions of this artificial neural network model with selected experimental data from literature.

# New predictions
Make water content outcome predictions using unseen data set from process parameters of a natural gas dehydration unit.
