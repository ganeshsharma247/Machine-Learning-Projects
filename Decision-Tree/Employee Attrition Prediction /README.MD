# Employee Attrition Prediction using Decision Tree 🌳📊

## 📌 Problem Statement

Employee attrition (employees leaving a company) can lead to increased recruitment costs, productivity loss, and business disruption. Organizations need a reliable way to identify employees who are at risk of leaving so that retention strategies can be applied proactively.

---

## 🎯 Project Objective

Build a machine learning model to predict whether an employee is likely to leave the company based on demographic, job-related, and work environment factors.

---

## 📊 Dataset Information

* Source: IBM HR Analytics Employee Attrition Dataset (Kaggle)
* Total Records: 1,470 Employees
* Original Features: 35
* Processed Features: 44+ (after encoding categorical variables)

### Target Variable

* Attrition = 0 → Employee Stays
* Attrition = 1 → Employee Leaves

---

## 🎯 Problem Type

* Binary Classification

---

## ⚙️ Algorithm Used

* Decision Tree Classifier

### Model Parameters

* Criterion = Entropy
* Max Depth = 4
* Min Samples Split = 20
* Min Samples Leaf = 10
* Class Weight = Balanced

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* Matplotlib
* Scikit-learn

---

## 🚀 Project Workflow

1. Loaded IBM HR Attrition dataset
2. Removed unnecessary columns:

   * EmployeeNumber
   * EmployeeCount
   * Over18
   * StandardHours
3. Converted target variable (Attrition) into numerical values
4. Applied One-Hot Encoding on categorical features
5. Split dataset into training (80%) and testing (20%)
6. Trained Decision Tree Classifier
7. Predicted employee attrition
8. Evaluated model performance
9. Calculated feature importance
10. Visualized feature importance and decision tree

---

## 💻 Code Snippet

```python
model = DecisionTreeClassifier(
    criterion="entropy",
    max_depth=4,
    min_samples_split=20,
    min_samples_leaf=10,
    class_weight="balanced",
    random_state=42
)

model.fit(X_train, y_train)
y_pred = model.predict(X_test)
```

---

## 📈 Model Evaluation

### Accuracy

* Accuracy: 72.79%

### Confusion Matrix

```text
[[191  56]
 [ 24  23]]
```

### Classification Report

| Metric    | Stay (0) | Leave (1) |
| --------- | -------- | --------- |
| Precision | 0.89     | 0.29      |
| Recall    | 0.77     | 0.49      |
| F1-Score  | 0.83     | 0.37      |

---

## 📌 Top Important Features

The model identified the following factors as the most influential:

1. TotalWorkingYears
2. OverTime
3. Age
4. MonthlyIncome
5. NumCompaniesWorked
6. EnvironmentSatisfaction
7. WorkLifeBalance
8. DistanceFromHome

---

## 📊 Visualizations

### Feature Importance Plot

Shows the most important factors affecting employee attrition.

### Decision Tree Visualization

Displays how the Decision Tree makes decisions and classifies employees as likely to stay or leave.

---

## 🎯 Business Use Cases

* Employee Retention Programs
* HR Analytics
* Workforce Planning
* Talent Management
* Attrition Risk Monitoring

---

## 📌 Key Insights

* Employees working overtime are more likely to leave.
* Total working experience significantly influences attrition.
* Work-life balance and job satisfaction impact retention.
* Salary and career growth factors play an important role.

---

## 📌 Conclusion

Decision Tree Classification provides an interpretable approach for predicting employee attrition. Feature importance analysis helps HR teams understand key drivers behind employee turnover and take proactive actions to improve retention.

---

## 👨‍💻 Author

Ganesh Sharma
