# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the standard libraries.

2.Set variables for assigning dataset values.

3.Import linear regression from sklearn.

4.Assign the points for representing in the graph.

5.Predict the regression for marks by using the representation of the graph.

6.Compare the graphs and hence we obtained the linear regression for the given datas.

## Program:
```
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: P Janardhan
RegisterNumber:  212224040128
import numpy as np
import matplotlib.pyplot as plt
x = np.array(eval(input()))
y = np.array(eval(input()))
x_mean = np.mean(x)
y_mean = np.mean(y)
num = 0
deno = 0
for i in range(1,len(x),+1):
    num = num + (x[i] - x_mean) * (y[i] - y_mean)
    deno = deno + (x[i] - x_mean)**2
m = num/deno
b = (y_mean) - (m*x_mean)
y_prediction = (m*x) + b
plt.scatter(x,y)
plt.plot(x,y_prediction,c = "green")
plt.show()
```

## Output:
![image](https://github.com/user-attachments/assets/850a3189-ca44-4274-b249-9b282dd0fee2)

![image](https://github.com/user-attachments/assets/286f4de3-d2a1-40f8-b465-732ac316291b)



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
