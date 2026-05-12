# SGD-Classifier
## AIM:
To write a program to predict the type of species of the Iris flower using the SGD Classifier.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Load the Iris dataset and separate features and target labels.
  
2. Standardize the feature values using StandardScaler for better model performance.

3. Split the dataset into training and testing sets.

4. Train the SGD Classifier model using the training data.

5. Predict test data results and evaluate accuracy with classification report.


## Program:
```
/*
Developed by: N.Gowsalya
RegisterNumber:  212225230085

from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.linear_model import SGDClassifier
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import accuracy_score, classification_report

iris = load_iris()
X = iris.data
y = iris.target

scaler = StandardScaler()
X = scaler.fit_transform(X)

X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

model = SGDClassifier(max_iter=1000, random_state=42)
model.fit(X_train, y_train)
y_pred = model.predict(X_test)

print("Accuracy:", accuracy_score(y_test, y_pred))

print("\nClassification Report:\n", classification_report(y_test, y_pred))

*/
```

## Output:

<img width="567" height="275" alt="Screenshot 2026-05-12 114641" src="https://github.com/user-attachments/assets/dd2bc65c-ad8c-482a-b398-347cb4ae2cac" />






## Result:
Thus, the program to implement the prediction of the Iris species using SGD Classifier is written and verified using Python programming.
