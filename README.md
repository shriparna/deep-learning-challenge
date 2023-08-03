# Module 21: deep-learning-challenge

## Author: Shridhar Kamat.
<hr>

### Details of the program 
#### Shridhar Kamat
#### Date: 8/03/2023
<hr>
Package Contents:

1. [DeepLearningModel/AlphabetSoupCharity.ipynb](https://github.com/shriparna/deep-learning-challenge/blob/main/DeepLearningModel/AlphabetSoupCharity.ipynb) Main Google Colab file to be evaluated. Need to run on Google Collab

2. [DeepLearningModel/AlphabetSoupCharity.h5](https://github.com/shriparna/deep-learning-challenge/blob/main/DeepLearningModel/AlphabetSoupCharity.h5) HDF5 file output from #1 above to be evaluated
#### Note: File may be too large to view

3. [DeepLearningModel/AlphabetSoupCharity_Optimization.ipynb](https://github.com/shriparna/deep-learning-challenge/blob/main/DeepLearningModel/AlphabetSoupCharity_Optimization.ipynb) Main Google Colab file with optimized model to be evaluated. Need to run on Google Collab

4. [DeepLearningModel/AlphabetSoupCharity_Optimization.h5](https://github.com/shriparna/deep-learning-challenge/blob/main/DeepLearningModel/AlphabetSoupCharity_Optimization.h5) HDF5 file output after optimization from #3 above to be evaluated
#### Note: File may be too large to view

<hr>

## Instructions:

- Download the Jupyter Notebook files from Github
- Open Google Collab
- Use File > Upload Notebook
- Upload file AlphabetSoupCharity.ipynb
- Execute from top to bottom
- Verify the evaluation results (Loss and Accuracy)
- Evaluate file AlphabetSoupCharity.h5 which is generated from above file
- Use File > New Notebook > Upload Notebook
- Upload file AlphabetSoupCharity_Optimization.ipynb
- Execute from top to bottom
- Verify the evaluation results (Loss and Accuracy)
- Evaluate file AlphabetSoupCharity_Optimization.h5 which is generated from above file
- The report is part of this document below:

<hr>

# Neural Network Model Report

## Overview

* Purpose of the analysis is to build a model for a notprofit foundation Alphabet Soup Company that can predict which applicants they can approach for funding with the best chance of success in their ventures. We fed the historical data of the applicants such as Application Type, Affiliation, Classification, Use Case, Organization, Status, Income Amout, Special Concideration and the Amount they funded earlier.

## Results

* Data Processing 
  * What variable(s) are the target(s) for your model?

    IS_SUCCESSFUL
  * What variable(s) are the features for your model?

    APPLICATION_TYPE,	AFFILIATION,	CLASSIFICATION,	USE_CASE,	ORGANIZATION,	STATUS,	INCOME_AMT,	SPECIAL_CONSIDERATIONS,	ASK_AMT	

  * What variable(s) should be removed from the input data because they are neither targets nor features?

    EIN,	NAME	

* Compiling, Training, and Evaluating the Model
  * How many neurons, layers, and activation functions did you select for your neural network model, and why?

    Started with 2 hidden layers with 80 and 30 neurons respectively. There were about 40+ input dimentions were there so wanted to double the size for the neurons for the first layer. In the next trials, tried to adjust it with more hidden layers, reducing neurons, changing the models etc.

  * Were you able to achieve the target model performance?

    No, but came close

  * What steps did you take in your attempts to increase model performance?

    Tried to increase the hidden layers, adjusted the neurons, tried with different activation, cut down on data


## Summary
Based on above data, here are our recommendations:
* We had the best result when we used the 2 hidden layers with 'Adam' optimizer
* In future, based on additional data that we receive the model may need to be retrained and reevaluated further
