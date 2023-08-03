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

* Purpose of the analysis is to build a model for a notprofit foundation Alphabet Soup Company that can predict which applicants they can approach for funding with the best chance of success in their ventures. We fed the historical data of the applicants such as Application Type, Affiliation, Classification, Use Case, Organization, Status, Income Amout, Special Concideration and the Amount they donated earlier.

## Results

* Data Processing 
  * For this Model1 we have the following scores:

* Compiling, Training, and Evaluating the Model
  * For this Model1 we have the following scores:

## Summary
Based on above data, here are our recommendations:
* We had the best result when we used the 2 hidden layers with 'Adam' optimizer
* In future, based on additional data that we receive the model may need to be retrained and reevaluated further
