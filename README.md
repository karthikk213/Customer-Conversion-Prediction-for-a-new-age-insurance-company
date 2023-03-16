# Customer-Conversion-Prediction-for-a-new-age-insurance-company

### Problem Statement
The insurance company wants to identify the customers who are most likely to convert so that they can be specifically targeted via call. For this purpose, historical marketing data of the insurance company is provided to build a machine learning model that will predict if a client will subscribe to the insurance.

### Dataset
The historical sales data is available as a compressed file in the data folder. The dataset consists of the following features:

age (numeric)
job : type of job
marital : marital status
educational_qual : education status
call_type : contact communication type
day: last contact day of the month (numeric)
mon: last contact month of year
dur: last contact duration, in seconds (numeric)
num_calls: number of contacts performed during this campaign and for this client
prev_outcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")
And the output variable (desired target):

y - has the client subscribed to the insurance?

### Solution
We approached the problem in the following manner:

Data preprocessing and cleaning
Handling imbalanced dataset
Feature selection and engineering
Model training and selection
Model evaluation using AUROC metric

****The important features that contribute towards the subscription of the insurance are 'age', 'day', 'dur', 'num_calls', 'job_blue-collar', 'job_entrepreneur', 'job_housemaid', 'job_management', 'job_retired', and 'job_self-employed'.****

****The XGBoost classifier performed the best with an AUROC score of 89%. Stratified sampling was used to ensure the class distribution is representative of the overall population.*****
