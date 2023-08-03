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

4. [DeepLearningModel/AlphabetSoupCharity.h5](https://github.com/shriparna/deep-learning-challenge/blob/main/DeepLearningModel/AlphabetSoupCharity.h5) HDF5 file output from #3 above to be evaluated

#### Note: File may be too large to view

<hr>

## Instructions:

- Activate PythonData environment using conda activate PythonData
- Download the file credit_risk_classification.ipynb
- Change directory to Credit_Risk
- Open Jupyter Notebook using command jupyter notebook
- Open the file credit_risk_classification.ipynb from the notebook
- Execute from top to bottom   
- The answers to the questions are part of the credit_risk_classification.ipynb using markdown
- The report is part of this document below:

<hr>

# Credit Risk Analysis Report

## Overview of the Analysis

* Purpose of the analysis is to build a model that can identify the credit worthiness of borrowers for a peer-to-peer lending services company based on a historical dataset of lending activities
* From the historical data, we can get the loan size,	interest rate, borrower income,	debt to income ratio,	num of accounts, derogatory marks, total debt and then to predict its credit worthiness as either `0` for a healthy loan versus `1` for a high risky loan
* Based on the historical data it was observed that there were approximately about 30 times `0` healthy loans compared to `1` high risk loans. 
* To understand it we need to first create a model, train the model using fit and then predict the model to determine the credit worthiness of the borrower by classifying it as `0` (healthy loan) and `1` (high-risk loan)
* For this we first used `LogisticRegression` which is used for classification models since the prediction to be made here is only two categories as `0` (healthy loan) or `1` (high-risk loan). But since the data was more for healthy loan (`0`), we were not getting expected results so we used random over sampling method to generate more sample data to balance out this difference. Once the sample size was balanced then we used the `LogisticRegression` again to get more better results.

## Results

The follwing details provide balanced accuracy scores and the precision and recall scores of the machine learning models we used.

* Machine Learning Model 1: `LogisticRegression` before random sampling 
  * For this Model1 we have the following scores:
    * Accuracy: **0.9442676901753825**
    * Precision: **100%** for Healthy Loan (`0`) and **87%** for High-Risk Loan (`1`)
    * Recall: **100%** for Healthy Loan (`0`) and **89%** for High-Risk Loan (`1`)

* Machine Learning Model 2: `LogisticRegression` after random sampling 
  * For this Model1 we have the following scores:
    * Accuracy: **0.9959744975744975**
    * Precision: **100%** for Healthy Loan (`0`) and **87%** for High-Risk Loan (`1`)
    * Recall: **100%** for Healthy Loan (`0`) and **100%** for High-Risk Loan (`1`)

## Summary
Based on above data, here are our recommendations:
* Model2 performed better as we can see that the Accuracy, Precision and Recall scores have been improved 
* Here the main focus should be on the High-Risk Loans (`1`) as we have historically good data for Healthy Loans (`0`) also its less risky but we now have improved score of High-Risk (`1`) using random over sampling
* Although the data is improved with Model2, it would be a business decision to determine if they are better off with the prediction of high-risk loans (`1`) as that is the most crucial risk at this time which was improved by random sample data but not the actual data
