# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import NumPy and DecisionTreeClassifier from sklearn.
2. Create the input data (Age and Years of Experience) and output data (Employee Churn).
3. Train the Decision Tree Classifier using the fit() function.
4. 1. Predict whether the employee will leave or stay using the predict() function and display the result.

## Program:
```py

import numpy as np
from sklearn.tree import DecisionTreeClassifier

X = np.array([[25, 1], [30, 2], [35, 3], [40, 5], [45, 6], [28, 1], [50, 7], [38, 4]])
Y = np.array([0, 0, 0, 1, 1, 0, 1, 1])

model = DecisionTreeClassifier(random_state=42)
model.fit(X, Y)

prediction = model.predict([[42, 6]])

if prediction[0] == 1:
    print("Employee will Leave")
else:
    print("Employee will Stay")

```

## Output:
<img width="170" height="43" alt="image" src="https://github.com/user-attachments/assets/f9800955-b00e-459b-8610-2871eb919ff0" />


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
