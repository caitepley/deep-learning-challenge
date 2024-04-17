# Analysis of Alphabet Soup Neural Net

## Overview
The purpose of this assignment is to analyze a dataset for the nonprofit foundation Alphabet Soup that contains details about funding applications and their success/failure. The goal is to use a neural net to help select applicants for funding that have the best chance of success. 

## Results

### Data Preprocessing:
- The target variable for the model is 'IS_SUCCESSFUL' because we are trying to teach to model to identify the characteristics of the applicants who succeed.
- The feature variables for the model are 'APPLICATION_TYPE','CLASSIFICATION','USE_CASE','STATUS','INCOME_AMT','SPECIAL_CONSIDERATIONS', and 'ASK_AMT'.
- 'NAME' and 'EIN' should be removed from the input data because they are not useful either as targets or as features. 

### Compiling, Training, and Evaluating the Model:
- I tried using 3 layers with 80, then 60, then 10 neurons. The first activation function was relu, and then I used tanh for the inner layers, and the sigmoid function to produce the output. I chose this because I wanted to see how adding a layer and changing the activation function would alter the output.
- None of the attempts I made achieved the model performance. 
- I tried adding another layer, changing the number of nodes, dropping more columns from the features, and changing the activation function. 

### Summary:
The results of the deep learning model are not ideal. The model was only able to achieve approximately 72.9% accuracy, which is not good when attempting to determine who to loan large sums of money to. K-Means with Principal Component Analysis could be used to solve this problem by determining which features affect the outcome the most and then plotting visible clusters to predict which applications would be successful.