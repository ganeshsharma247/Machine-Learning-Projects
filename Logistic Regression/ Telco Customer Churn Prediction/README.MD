# Telco Customer Churn Prediction 📉📊

## 📌 Problem Statement

Telecommunication companies lose significant revenue due to customer churn.
Identifying customers likely to leave helps in taking proactive retention actions like offers, discounts, and personalized services.

---

## 🎯 Project Objective

Build a machine learning model to predict whether a customer will churn (leave the service) based on demographic, service, and billing data.

---

## 📊 Dataset Information

* Source: Telco Customer Churn Dataset

### Features:

* Demographics → Gender, SeniorCitizen, Partner, Dependents
* Account Info → Tenure, Contract type
* Services → PhoneService, InternetService, Streaming services
* Billing → MonthlyCharges, TotalCharges, PaymentMethod

### Target:

* Churn

  * 0 → No churn
  * 1 → Churn

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
2. Removed irrelevant column (`customerID`)
3. Converted target variable (Yes/No → 1/0)
4. Applied Label Encoding on categorical features
5. Split dataset using stratified sampling (80% train, 20% test)
6. Trained Logistic Regression model
7. Predicted churn on test data
8. Evaluated model using:

   * Confusion Matrix
   * Precision, Recall, F1-score

---

## 💻 Code Snippet

```python id="ch1x9a"
model = LogisticRegression(max_iter=10000)
model.fit(X_train, y_train)

y_pred = model.predict(X_test)
```

---

## 📈 Model Evaluation

### Confusion Matrix

```
[[925 110]
 [177 197]]
```

### Classification Report (Key Metrics)

* Accuracy: **0.80 (80%)**
* Precision (Churn=1): **0.64**
* Recall (Churn=1): **0.53**
* F1-score: **0.58**



## 📌 Key Insights

* Model performs well on non-churn customers
* Recall for churn class is moderate → some churn customers are missed
* Improving recall is important for better retention strategies



## 🎯 Business Use Cases

* Target at-risk customers with retention offers
* Reduce revenue loss due to churn
* Improve customer satisfaction


## 📌 Conclusion

Machine Learning helps identify potential churn customers.
Improving recall for churn cases can significantly enhance business impact.



## 👨‍💻 Author

Ganesh Sharma
