# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import panda
### Step2
import linear model from sklearn
### Step3
read the file cars.csv
### Step4
assign the values for x and y as required
### Step5
create the linearregression model and predict the output
## Program:
```
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('employee.csv')

x = df[['experience','education']]
y = df['salary']

regr = linear_model.linearregression()
regr.fit(x,y)

print("coefficient:",regr.coef_)
print("interept:", regr.intercept_)

new_employee = [[5,2]]
predicted_salary = regr.predict(new_employee)

print("predicted salary for the corresponding experience and education:",predicted_salary)
```
## Output:
![Screenshot 2024-01-02 200341](https://github.com/Harishragaventhira/Multivariate-Linear-Regression/assets/145548269/759aadb7-4d80-4915-9a54-095380bde0fb)
![Screenshot 2024-01-02 200355](https://github.com/Harishragaventhira/Multivariate-Linear-Regression/assets/145548269/0ad02a33-ca32-4368-bd1e-97a065f0d82e)
![Screenshot 2024-01-02 200415](https://github.com/Harishragaventhira/Multivariate-Linear-Regression/assets/145548269/2da19a38-1bb2-487f-9b26-dc5db2713d5b)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
