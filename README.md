# Neural Network Charity Analysis

## Overview of the analysis
The purpose of this analysis is to make predictions about which organizations Alphabet Soup Charity should and should not make investments into based on previous data.

## Results 

### Data Preprocessing
- The target variable for this analysis is the column 'IS_SUCCESSFUL'
- The feature variables for this analysis are the columns ‘APPLICATION_TYPE’, ‘AFFILIATION’, ‘CLASSIFICATION’, ‘USE_CASE’, ‘ORGANIZATION’, ‘STATUS’, ‘INCOME_AMT’, ‘SPECIAL_CONSIDERATIONS’, and ‘ASK_AMT’
- The variables that are neither targets nor features and were removed from the input data were 'EIN' and 'NAME'

### Compiling, Training, and Evaluating the Model
- In the initial model, there were two hidden layers
  - Layer one had 80 neurons
  - Layer two had 30 neurons
- Layer one and layer two had a Relu activation function
- The output layer had one neuron and a Sigmoid activation function
- Using this model, I was unable to achieve the target model performance of +75% accuracy

- In my later models, I tried to increase the accuracy to achieve the target model performance of +75%
- I did so by:
  - Dropping another column, 'ASK_AMT'
  - Increasing the epochs from 100 to 150
  - Adding more neurons to the hidden layers, increasing 80 to 100 and 30 to 40
- I was still unable to increase the model performance accuracy to exceed 75%


## Summary: 
Overall, my deep learning model did not achieve a high degree of accuracy. I was unable to achieve the target model performance of +75% accuracy. For future analysis, I would recommend a different type of machine learning model, such as supervised machine learning that can better handle this type of binary classification.
