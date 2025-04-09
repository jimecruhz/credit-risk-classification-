# Module 12 Report 

## Overview of the Analysis

* **Purpose of the analysis** - The goal of this determine if the logistic Regression machine learning model can more accurately predict healthy loans versus high-risk loans using the original dataset or a dataset that is resampled to increase the size of the minority class

* - **The Dataset** - The dataset used to perform the analysis consist of information on 77,536 loans. The data includes columns for loan_size, interest_rate, borrower_income, debt_to_income ratio, number_of_accounts, derotory_marks, total_debt, and loan_status. The category what we are attempting to predict wit our analysis is **loan_status**. The data provided in the remaining columns willl be used as features to train the data and inform the predictions. 
*  **Stages of the Machine Learning Process**  - The stages of the machine learning process are very scripted. It followed in order, they provide you with an accurate assessment of the model's ability to make predictions. The stages of the machine learning process are as follows: 
	* Prepare the data -  import the file, establish the DataFrame, evaluate the columns and features. 
	* Separate the data into features and labels - The labels are what you are attempting to predict, is the status of the loan healthy (0) or high-risk (1). The feature are all of the remaining data you will use to train and test the model. 
	* Use the train_test_split function to separate the features and labels data into training and testing datasets. 
	* import the machine learning model from the library - In this instance, we will be importing LogisticRegression from SKLearn

**Machine Learning Method Utilized** - 
The Primary model used in the analysis is: 
* LogisticRegression model from SKLearn 
Supporting functions used in this analysis are: 
	- train_test_split from SKLearn
	
Models are evaluated using the following functions: 
-confusion_matrix from SKLearn
-classification_report from SKLearn

	

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model - Logistic Regression: 
    * **Accuracy Score** 99% 
    * **Precision Score** 
	    * Class 0 (Healthy  Loans): 100% 
	    * Class 1 (High-risk Loans) : 85%
	 * **Precision Score** 
	    * Class 0 (Healthy  Loans): 99% 
	    * Class 1 (High-risk Loans) : 91%

## Summary

The model does a great job in using the original data to predicting the value of the healthy loans. Precision was 100% and recall was 99%.
 
 The model is pretty good at predicting the values of high risk loans, but not as good as predicting the healthy loans. Precision was 85% and recall was 91%. 

Given this information, it appears that the Logistic Regression model does a great job at predicting both healthy and high-risk loans, given the features that are used to train the data. 
