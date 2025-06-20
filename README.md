# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd

### Step2
Read the csv file
### Step3
Get the value of x and y variables
### Step4
Create the linear regression model and fit


### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.


## Program:
```
#Developed by: Ganga devi  
#Register number:212224240042

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```






## Output:
![Screenshot 2025-06-09 100533](https://github.com/user-attachments/assets/3d54f1f9-c06e-49fe-9499-d00acf229024)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
