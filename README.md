# Neural Network Charity Analysis

## Overview

The purpose of this analysis is to explore the application of TensorFlow Keras in Python to be able to construct a neural network that would be able to identify if charity candidates would be successful given a dataset including various specifications of successful and unsuccessful charities. 

## Results

The primary target variable is seen in the "IS_SUCCESSFUL" column, which already is process as 1 or 0 for a success or failure. In such analysis, the names or identifiers are deemed not necessary to the success and are dropped from as a feature for the model.

The initial attempt for the model included two hidden layers with 80 and 30 neurons respectively - each using the ReLU activation function. 

In the optimization attempt, four hidden layers were used at 120, 120, 80, and 30 neurons respectively. In this attempt, Leaky ReLU was used as the activation function, with double the epochs. 

## Summary
The initial attempt yielded the folllowing loss and accuracy: 
![Initial](/screenshots/initial.png)

The subsequent optimization attempt yielded as such: 
![Optimization](/screenshots/optimization.png)

We find that the loss was marginally improved with our changes; however, the impact to accuracy was not significant. At these percentages, it may be a good strategy to reattempt a model using Random Forest or an SVM to create a model.
