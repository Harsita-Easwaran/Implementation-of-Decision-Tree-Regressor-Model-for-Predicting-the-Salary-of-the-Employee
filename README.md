# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Harsita Easwaran
RegisterNumber:  24013629
*/
```
import pandas as pd
data=pd.read_csv("Salary.csv")
data. head () 
data. info()
data.isnull().sum() 
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder ()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data["Salary"]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor 
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
y_pred
r2=r2_score (y_test,y_pred)
print("R2 score:",r2)
dt.predict([[5,6]])
## Output:
![Decision Tree Regressor Model for Predicting the Salary of the Employee](sam.png)
![Screenshot 2024-11-28 235209](https://github.com/user-attachments/assets/9bd4b20a-c696-45d7-ad19-49e8af1e4ba5)
![Screenshot 2024-11-28 235217](https://github.com/user-attachments/assets/631b7af5-7987-4533-8579-3671c1645071)
![Screenshot 2024-11-28 235225](https://github.com/user-attachments/assets/02542010-a34a-4d86-bb35-bbe44d9087e5)
![Screenshot 2024-11-28 235232](https://github.com/user-attachments/assets/eb50d586-e49b-41fb-a861-318950775683)
![Screenshot 2024-11-28 235239](https://github.com/user-attachments/assets/66337efd-8d8e-409b-9771-dfa69d2756d6)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
