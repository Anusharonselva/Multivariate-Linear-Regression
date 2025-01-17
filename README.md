# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 Import Pandas library.
### Step2 Import Linear_model from sklearn.
### Step3 Read the csv file using pandas library.
### Step4 Enter the parameters of the linear function.
### Step5 Print the parameters of the linear function. End the program.


## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/cars (1).csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient",regr.coef_)
print("Intercept",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)






```
## Output:
### Insert your output
![exp-10 maths ai 1](https://github.com/Anusharonselva/Multivariate-Linear-Regression/assets/119405600/b42167b0-d8d7-4c65-a3b6-26dcc31728b7)


![exp-10 maths ai 2](https://github.com/Anusharonselva/Multivariate-Linear-Regression/assets/119405600/384623c2-5a6b-4654-8301-22ceabf6464f)



<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
