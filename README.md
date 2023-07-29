# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.
<br>

### Step2
<br>
Import linear_model from sklearn.

### Step3
Open the file in read mode.
<br>

### Step4
Using LinearRegression() print its coefficients and intercept.
<br>

### Step5
Using predicted() print the predicted output for the given values.

<br>

## Program:


```
#Implementation of Multivariate Linear Regression
# Developed by: POPURI SRAVANI
# Register Number: 23006561
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('cars.csv')
x=df[['Weight','Volume']]
y=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("coefficients:",regr.coef_)

print("Intercept:",regr.intercept_)
predictedco2=regr.predict([[4500,2300]])
print("predicted co2 for the corresponding weight and volume",predictedco2)


```
## Output:
<br>

### Insert your output


![Alt text](<2023-07-26 (3).png>)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.