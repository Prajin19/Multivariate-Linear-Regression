# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas library.

### Step2
Import Linear_model from sklearn.


### Step3
Read the csv file using pandas library.


### Step4
Enter the parameters of the linear function.

### Step5
Print the parameters of the linear function.

## Program:
```
import pandas as ps
from sklearn import linear_model
data=ps.read_csv("crse.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predict=regr.predict([[3300,1300]]) 
print('Predicted CO2 for for the corresponding weight and volume',predict)
```
## Output:

![Screenshot 2023-12-26 145856](https://github.com/Prajin19/Multivariate-Linear-Regression/assets/144979377/596151d1-12e0-4e21-a5d3-95901879b3fb)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
