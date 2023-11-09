# Deep Learning Project

## Overview of the Analysis

Alphabet Soup, a nonprofit foundation, aims to make data-driven decisions when selecting applicants for funding, seeking to identify those with the highest chances of success in their ventures. The goal of this project is to create a binary classifier using machine learning and neural networks. This classifier will predict whether applicants will be successful if funded by Alphabet Soup. The foundation has provided a dataset containing information on over 34,000 organizations that have received funding.

The variables I aimed to predict included 'value_counts,' a metric utilized to ascertain the count of unique values within each data point. When the count exceeded 10, rare categorical variables were grouped into bins. Subsequent to data preprocessing, I proceeded to compile, train, and assess the binary classification model, thereby determining the model's performance through the measurement of loss and accuracy.

## Results

  Data Preprocessing
    * The target variables of the model was [IS_SUCCESSFUL]
    * The feature variables of the model were ['APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT'])
    * The variables removed from the input were ['EIN', 'NAME']

  Compiling, Training, and Evaluating the Model
    
* Machine Learning Model 1:
  * The Model 1 2 hidden layers. The first hidden layer had 90 neurons and the second, 30. The ReLU function was used due to it's simplicity and effectiviness. 
  * The accuracy of this model was 72.89%.

* Machine Learning Model 2:
    * In this model, it was increased the number of neurons in each layer. The first hidden layer had 98 neurons and the second, 49. The activation function was also modified to Tanh, in order to produce an output that ranges from -1 to 1.
    * It was created more bins to the rare occurance in the columns [APPLICATION_TYPE] and [CLASSIFICATION]. 
    * The accuracy of this model was 73.07%.
  
* Machine Learning Model 3:
    * In this model, it was increased the number of neurons in each layer. The first hidden layer had 120 neurons and the second, 60. The activation function remained Tanh.
    * The accuracy of this model was 73.15%.


## Summary

  While Model 3 achieved a higher accuracy than Model 2, it also exhibited an increased loss. As a result, none of the models generated in this project are recommended. In this context, the model's performance is not contingent on the specific problem being addressed, as the primary focus is on predicting the positive class (1).
