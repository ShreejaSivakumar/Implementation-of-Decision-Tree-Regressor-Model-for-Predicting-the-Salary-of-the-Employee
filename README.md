# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

# EXPT : 09

# NAME : SHREEJA R S
# REF.NO : 25017561

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm


1. **Load** → Read `Salary.csv` and separate features (X) and target salary (y)
2. **Encode** → Convert categorical text columns into numeric format
3. **Split** → Divide data into 80% training and 20% testing sets
4. **Train** → Fit the Decision Tree Regressor on training data
5. **Evaluate** → Measure performance using MAE, MSE, and R² Score
6. **Visualize** → Plot, save, and display the Decision Tree image

---


## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SHREEJA R S
RegisterNumber: 25017561


import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeRegressor, plot_tree
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score

# 1. Load the dataset
data = pd.read_csv("Salary.csv")

# 2. Separate features and target
X = data.drop("Salary", axis=1)
y = data["Salary"]

# 3. Encode categorical columns
X = pd.get_dummies(X, drop_first=True)

# 4. Split into training and testing sets
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

# 5. Train the Decision Tree Regressor
model = DecisionTreeRegressor(random_state=42)
model.fit(X_train, y_train)

# 6. Predict and Evaluate
y_pred = model.predict(X_test)

print("Mean Absolute Error :", mean_absolute_error(y_test, y_pred))
print("Mean Squared Error  :", mean_squared_error(y_test, y_pred))
print("R² Score            :", r2_score(y_test, y_pred))

# 7. Visualize the Decision Tree
plt.figure(figsize=(25, 12))
plot_tree(
    model,
    feature_names=X.columns.tolist(),
    filled=True,
    rounded=True,
    fontsize=8
)
plt.title("Decision Tree Regressor - Salary Prediction")
plt.tight_layout()
plt.savefig("decision_tree_regressor.png", dpi=150)
plt.show()


*/
```

## Output:


<img width="1240" height="692" alt="Screenshot_13-5-2026_135323_localhost" src="https://github.com/user-attachments/assets/35d77053-7f17-44af-b06c-6f6cc228f2fb" />


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.
V



























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.




























































..........
..
.
.
.
...
.
.
.
..
.
..
.
..
.
.
.
.
.
.

.
.
.
.
.
.
..

.
.
.
