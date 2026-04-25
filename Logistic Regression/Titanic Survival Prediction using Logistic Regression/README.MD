# Titanic Survival Prediction using Logistic Regression 🚢📊

## 📌 Project Objective

The objective of this project is to predict whether a passenger survived the Titanic disaster based on features like age, gender, class, and fare.

---

## 📊 Dataset Information

* Source: Kaggle (Titanic Dataset)

### Features:

* Pclass → Passenger class
* Sex → Gender
* Age → Age of passenger
* SibSp → Number of siblings/spouses aboard
* Parch → Number of parents/children aboard
* Fare → Ticket fare
* Embarked → Port of embarkation

### Target:

* Survived

  * 0 → Did not survive
  * 1 → Survived

---

## 🎯 Problem Type

* Binary Classification

---

## ⚙️ Algorithm Used

* Logistic Regression

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* Scikit-learn

---

## 🚀 Project Workflow

1. Loaded dataset using Pandas
2. Selected relevant features and target variable
3. Handled missing values using SimpleImputer
4. Applied feature scaling (StandardScaler) for numerical data
5. Applied One-Hot Encoding for categorical data
6. Created preprocessing pipeline using ColumnTransformer
7. Built full pipeline with Logistic Regression model
8. Split dataset into training (80%) and testing (20%)
9. Trained model using pipeline
10. Evaluated model using accuracy, confusion matrix, and classification report
11. Predicted survival for new passenger data


## 💻 Code Snippet

```python id="t9plx2"
lrPipe = Pipeline([
    ("preprocessor", preprocessor),
    ("classifier", LogisticRegression(max_iter=1000))
])

lrPipe.fit(X_train, y_train)
y_pred = lrPipe.predict(X_test)
```


## 📈 Model Evaluation

* Accuracy Score
* Confusion Matrix
* Classification Report

---

## 📌 Key Insights

* Gender and passenger class strongly influence survival
* Data preprocessing significantly improves model performance
* Pipelines make the workflow clean and reusable

---

## 🎯 Use Cases

* Survival prediction systems
* Data preprocessing pipelines in ML projects
* Real-world classification problems

---

## 📌 Conclusion

Using a pipeline with preprocessing and Logistic Regression improves accuracy and ensures a clean, scalable machine learning workflow..

---

## 👨‍💻 Author

Ganesh Sharma
