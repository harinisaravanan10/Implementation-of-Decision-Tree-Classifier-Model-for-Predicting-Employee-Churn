# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas
2.Import Decision tree classifier
3.Fit the data in the model
4.Find the accuracy score 

## Program:


```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Harini S
RegisterNumber:  212223040058


import pandas as pd

data = pd.read_csv("Employee.csv")

data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()

data["salary"] = le.fit_transform(data["salary"])
data.head()

x=data[["satisfaction_level","last_evaluation","number_project", "average_montly_hours",
"time_spend_company", "Work_accident","promotion_last_5years","salary"]]
x.head()

y = data["left"]

from sklearn.model_selection import train_test_split
x_train, x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn. tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt. predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)

accuracy
dt.predict([[0.5,0.8,9,260, 6,0,1,2]])
*/
```

## Output:

<img width="1232" height="228" alt="390815135-0a4fa5db-4d79-4ebd-9926-f4d1ee83d1e3" src="https://github.com/user-attachments/assets/81431be8-1fed-4cd3-a0d8-babdbc97be9d" />
<img width="980" height="366" alt="390815192-ea8d6d09-3cc4-4875-ade1-46c9aa59e5c0" src="https://github.com/user-attachments/assets/232529a7-4802-45f9-8332-3fc0cce1c52e" />
<img width="843" height="257" alt="390815252-9b850bb3-7c7e-4775-b2e3-789789375431" src="https://github.com/user-attachments/assets/0d00a524-5e82-4650-916c-2161214f1f8e" />
<img width="501" height="120" alt="390815439-7b31af4d-1ce9-4ff7-b45c-938ce231cb83" src="https://github.com/user-attachments/assets/88ede28e-579e-4309-b811-cbc982114de8" />
<img width="1247" height="223" alt="390815519-71654c7d-2c86-4613-8d03-a010cb8a2b11" src="https://github.com/user-attachments/assets/ef2a660b-f8e1-4cca-87b9-f4e889c1e87a" />
<img width="1226" height="222" alt="390815584-5442db03-d63b-404e-ab1f-d9552a1a6a83" src="https://github.com/user-attachments/assets/3a0da490-2700-42a3-8ddf-75da12fee890" />
<img width="452" height="65" alt="390815637-727ed6aa-319b-4a29-8147-e094729d5549" src="https://github.com/user-attachments/assets/9589aeea-dfc9-425f-a598-7eceac8f5a2f" />
<img width="651" height="482" alt="390815766-4d27bab8-fef9-46a9-869c-23296ad3caac" src="https://github.com/user-attachments/assets/0eeabfba-06f2-470b-b1e0-ee5928d8ae8e" />

RESULT:

Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
