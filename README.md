# EX-07 Implementation of Decision Tree Regressor Model for Predicting the Salary of the Employee
### Aim:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
### Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook
### Algorithm
1. Import pandas and read the csv file.
2. Encoding the data and Import Decision tree classifier.
3. Fit the data in the model.
4. Find the MSE , r2 and the Predicted.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: BALAMURUGAN B
RegisterNumber: 212222230016
import pandas as pd
data=pd.read_csv('Salary.csv')
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,7]])

*/
```

## Output:

### DATASET
![head](https://github.com/BALA291/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/120717501/143f556a-dd4b-4ce6-86c7-0a743bab3da4)

### INFO
![info](https://github.com/BALA291/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/120717501/d969fcf7-f1c8-41fd-bcb1-26e830e76d61)

### NULL VALUES
![null](https://github.com/BALA291/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/120717501/8a75c87d-4592-4788-ab0f-2fcc5a0a5891)

### LABEL ENCODING
![label](https://github.com/BALA291/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/120717501/3dc772d7-047a-43c0-a3b7-9de21399fa6b)

### MSE
![mse](https://github.com/BALA291/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/120717501/a865ce83-381c-41ae-baf0-b3323f8d6d95)

### R2
![r2](https://github.com/BALA291/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/120717501/eb727452-5b0e-48a9-9b84-1827ebbfef8f)

### PREDICTED VALUE
![predict](https://github.com/BALA291/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/120717501/8c091781-1efb-4c14-950f-4a6cc7eb6346)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
