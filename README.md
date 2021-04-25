# Prediction-of-water-content-outcomes-in-gas-dehydration-systems-using-AI
An artificial neural network model was created to predict the water content outcomes of natural gas dehydration systems. 


# Summary
Natural gas suppliers have a strict water content limit of 7 lbs/MMscf to meet. Gas with water content value above this allowable limit is tagged off-spec and a lower monetary value is placed on it.

This project is an artificial neural network model used for predicting the water content outcomes of a natural gas dehydration system. The water content outcomes are either class 0 or class 1.

Class 0 represents data points that meet the sales gas pipeline quality water content specification of 7 lbs/MMscf and class 1 represents data points that do not meet the sales gas pipeline quality water content specification of 7 lbs/MMscf.

The training, validation and test data used is: Hernandez-Valencia et al., (1992) which has 2020 data points. 985 are class 1, 1035 are class 0.

The model was further evaluated with experimental data from literature (Arubi & Duru, 2008).  

# Data used
The source of the data is secondary data from the work of Hernandez-Valencia et al., (1992) where a TEG dehydration unit was modeled with PROSIM software.
The data consists of four input features and one target output used in training and testing the artificial neural network model. The features are TEG recirculation rate (represented as TEG_recirc_rate), number of equilibrium stages (represented as no_of_equili_stages), temperature of the reboiler (represented as temp), and stripping gas flow rate (represented as stripping_rate). 

# Exploratory Data analysis (EDA)
Exploratory data analysis is important for any artificial neural network model because the strength of the model prediction is partly dependent on the data, amongst other things.

An EDA was carried out on the training data used in building the artificial neural network model. The EDA show the effects of varying the dehydration process parameters on the dehydration process parameters and water content outcome and invariably the expected water content outcomes of new dehydration process parameters.

It also shows the optimum value for each dehydration process parameters to ensure the water content specification is met. 
All statistics calculation was carried out with the Pandas library and all plots have been created with the Seaborn library in Python. 

# Model development
The ANN model was developed and fitted a three layer artificial neural network model with input features, reboiler temperature, number of equilibrium stages, triethylene glycol recirculation rate and stripping gas rate and output feature water content using back propagation method to minimize the error and Adam optimizer to optimize the weights. The hidden layer will contain seven nodes

# Model Evaluation
The model was evaluated and validated  for the model loss, accuracy, confusion matrix, precision score, recall score, and F1 score using independent validation dataset apart from the training data set.

# Evaluation with experimental literature data
Water content outcome predictions of this artificial neural network model were compared with selected experimental data from literature.

# New predictions
New predictions of water content outcome were made using unseen data set from process parameters of a natural gas dehydration unit.
