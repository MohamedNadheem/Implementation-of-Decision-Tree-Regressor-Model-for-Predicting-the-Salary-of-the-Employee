# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. importing libraries
2. reading data set
3. using label encoder
4. train and test the model
5. finging mse and metrics_score

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Mohamed Nadheem N
RegisterNumber:  212223240091
import pandas as pd
data=pd.read_csv('Salary.csv')
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
dt.predict([[5,6]])

*/
```

## Output:
## Data:
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742402/c5ded434-6b73-431d-8d48-d4fa2e4b4348)
## Label:
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742402/3c463e90-5443-46f2-8ca8-316e01c786f8)
## Mean Square Error:
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742402/20327990-d94f-49f0-8062-0f4d26aae812)
## Metrics Score:
![image](https://github.com/Jeshwanthkumarpayyavula/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742402/a3d5e9bd-892e-459a-bffe-2173e0a45ef1)







## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
