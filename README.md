# Credit-Risk-Classification-using-Logistic-Regression

The aim of this project is to analyze historical lending activity data to identify creditworthiness of creditors. The Reason of this analysis is to generate a model that will identify 'healthy loan' and 'high risk loan' applicants based on application factors which include loan size, interest rate, applicants income, debt to income ratio, number of accounts, pre-defined derogetory marks, and total debt.

## Initials

Python and softwares downloaded -

1. Python 3.10 or later
2. Anaconda Distribution
3. Pandas
4. scikit-learn

## Installation
1. Install the latest verion of Python here.

2. Install the latest version of Anaconda here.

3. Installing Anaconda includes the Pandas package.

4. To install the scikit-learn packages, run the following command in your terminal.

- pip install -U scikit-learn -

## Results 
* Machine Learning Model 1 (with original data):

Test Data Balanced Accuracy: 99%
Test Data Precision for 'healthy loans': 100%
Test Data Precision for 'high risk loans': 85%
Test Data Recall for 'healthy loans': 99%
Test Data Recall for 'high risk loans': 91%

* Machine Learning Model 2 (with resampled data):

Test Data Balanced Accuracy: 99%
Test Data Precision for 'healthy loans': 99%
Test Data Precision for 'high risk loans': 99%
Test Data Recall for 'healthy loans': 99%
Test Data Recall for 'high risk loans': 99%

## Overview of the Analysis
The first Logistic Regression model, using original data, did prediction of 'healthy loans' with accuracy, precision and recall close to 100%. It still does well, but performs noticably bad at identifying high-risk loans where it has a precision of 85% and a recall of 91%. This suggests that this model is less able to classify high risk loans than healthy loans. This is likely related to the skew in the data that was provided, with only about 3 percent of the sample being in the high risk loans category. The second Logistic Regression model that uses resampled data, performs noticably better at identifying high risk loans in addition to identifying healthy loans. The overall prediction rate is consistent across precision, recall, and accuracy. We would recommend utilizing the second model because of its heightened ability to detect 'high risk loans' accurately. This is especially important given how much it can cost a loan provider to misidentify and lend money to a 'high risk loan' applicant, and the minimal cost of misidentifying a 'healthy loan' applicant. The first model is slightly better at identifying 'healthy loan' applicants, but this is less important than correctly identifying 'high risk loan' applicants, which is accomplished better with the second model.
