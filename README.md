# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import libraries and load the dataset

### Step2
Prepare the data (features and target variable)

### Step3
Train the Linear Regression model

### Step4
Display the coefficients and intercept of the model

### Step5
Make prediction using the trained model

## Program:
```
develped by:G.T.GOWTHAM
reg no:212224110017


import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)






```
## Output:
![443061546-ebf0c3af-9543-4cc7-9bf0-58c3f5bf7481](https://github.com/user-attachments/assets/c3c2b752-b160-487f-aa95-61176aff29de)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
