Report
Overview
The goal of this project was to create a neural network model that could predict the success of an application for funding.
Results
Data Preprocessing:

Target variables
IS_SUCCESSFUL
Feature variables
APPLICATION_TYPE
AFFILIATION
CLASSIFICATION
USE_CASE
ORGANIZATION
STATUS
INCOME_AMT
SPECIAL_CONSIDERATIONS
ASK_AMT
Removed variables
EIN
NAME
Compiling, Training, and Evaluating the Model

For the initial model
2 hidden layers with relu activation and 30 total neurons.
Output layer of 1 neuron with sigmoid activation
Trained over 100 epochs
Tried to optimize performance and find a good starting point.
Relu activation was used because the dataset was positive numbers.
Sigmoid activation was used for the output to achieve a probability between 0 and 1.
Training on 100 epochs allowed a reasonable amount of tuning for the time needed to train.
Model performance
Inital model tested at 72.24% accuracy.
Optimization attempts never increased accuracy over 73% when tested.
Optimiation attempted by:
Removing the status variable
Having up to 4 hidden layers
Having up to 64 neurons in hidden layers
Changing various hidden layer activation functions to tanh or leaky relu
Changing the number of epochs between 20, 100, and 1000.
Summary
The highest accuracy obtained was still less than 73%. This is too unreliable to use as a model. I would next try to use logistic regression model. This model is suited for a binary output like success and failure of applications, and the model works well with scaled data.
