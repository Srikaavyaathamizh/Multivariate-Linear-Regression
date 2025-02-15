# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3

## Step6:
Print the predicted output.
## Program:
```
##Developed by: SRIKAAVYAA T
##Register number: 23013589

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("sricar.csv")
a=df[['Weight','Volume']]
b=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3400,1350]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)

```
## Output:
![Screenshot 2023-12-30 193430](https://github.com/Srikaavyaathamizh/Multivariate-Linear-Regression/assets/144870938/54390ecc-bb65-44b0-8c12-da4e72d5471a)



### Insert your output
```
Coefficient: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted CO@ for the corresponding weight and volume [115.90503767]
```

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
