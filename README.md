# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas

### Step2
Import linear model

### Step3
Read the csv file

### Step4
Enter the parameters to implement

### Step5
Run the program and predict the output

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predicted=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predicted)

```
## Output:

![Screenshot (96)](https://github.com/Jaiganesh235/Multivariate-Linear-Regression/assets/118657189/bade9dfe-e9c0-4787-9d11-5f57558819c8)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
