## CPI-Index-Prediction

The report is made for the individual assignment for USYD's unit - QBUS2820.

The Consumer Price Index (CPI) is a measure that examines the weighted average of prices of consumer goods and services, such as transportation, food, and medical care. It is calculated
 by taking price changes for each item in a predetermined basket of goods and averaging them. Changes in the CPI are used to assess price changes associated with the cost of living. The CPI is
 one of the most frequently used measures of inflation and deflation 1.
 
 In this project, your task is to develop a predictive model to forecast CPI of a particular sector given its historical quarterly values. The CPI data set CPI_train.csv contains the quarterly CPI data from Jan 1990 to Dec 2019 (120 data points). This data set is based on a real CPI dataset with some added noise for de-identification purposes. The test data set CPI_test.csv (not provided) has the same structure as the training data, and contains the quarterly CPI data from Jan 2020 to Dec 2021 (8 data points).
 
 Your task is to develop a predictive model, using CPI_train.csv, to forecast the quarterly CPI measures from Jan 2020 to Dec 2021. Note that, this is a multiple-step-ahead forecast problem.

 For the measure of forecast accuracy, please use mean squared error (MSE). The MSE, computed on the test data, is defined as follows. Let <img width="103" height="40" alt="image" src="https://github.com/user-attachments/assets/8586d1e5-d462-4fe1-9ec7-0b30fe324e85" /> be the h-step-ahead forecast of <img width="64" height="32" alt="image" src="https://github.com/user-attachments/assets/a4eac15c-4f3e-4518-8917-4d4e4a0bc9d1" />, based on the training data <img width="53" height="35" alt="image" src="https://github.com/user-attachments/assets/5be3831b-27bd-420a-a310-e067a622c341" />, where <img width="64" height="32" alt="image" src="https://github.com/user-attachments/assets/f424741f-5c43-42f1-9f0a-6534c78c612b" /> is the h-th value in the test data CPI_test.csv. The test error is computed as follows

<img width="503" height="108" alt="image" src="https://github.com/user-attachments/assets/149161c6-4632-4e5b-bec7-c77ef51335a8" />

where 8 is the number of observations in the test data.
