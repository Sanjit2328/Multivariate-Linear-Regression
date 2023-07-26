# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Importing pandas and scikit-learn libraries

### Step2
Reading the data from a CSV file

### Step3
Splitting the data into features (X) and target (y)

### Step4
Creating and fitting the linear regression model

### Step5
Printing the coefficients and intercept of the linear regression model:

### step6
Making a prediction

### step7
Printing the predicted CO2 emissions

## Program:
```python
#Developed by:Sanjit.P
#register number:23002570
import pandas as pd
from sklearn import linear_model

df=pd.read_csv("bmw.csv")
x= df[['Weight','Volume']]
y= df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictedCO2)






```
## Output:
![output](10.png)



<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.