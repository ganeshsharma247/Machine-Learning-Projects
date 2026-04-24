# Customer Purchase Prediction using Logistic Regression 🛒📊

## 📌 Project Objective

The objective of this project is to predict whether a customer will purchase a product after seeing an advertisement.

---

## 📊 Dataset Information

* Source: Kaggle (Social Network Ads Dataset)

### Features:

* Age → Age of customer
* EstimatedSalary → Customer salary

### Target:

* Purchased

  * 0 → Not Purchased
  * 1 → Purchased

---

## 🎯 Problem Type

* Binary Classification Problem

---

## ⚙️ Algorithm Used

* Logistic Regression

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* Scikit-learn
* Matplotlib

---

## 🚀 Project Workflow

1. Imported required libraries
2. Loaded dataset from Kaggle
3. Selected features (Age, EstimatedSalary)
4. Defined target variable (Purchased)
5. Split dataset into training (80%) and testing (20%)
6. Applied feature scaling using StandardScaler
7. Trained Logistic Regression model
8. Predicted results on test data
9. Evaluated model using accuracy score

---

## 💻 Code Snippet

```python id="lgx2p1"
model = LogisticRegression()
model.fit(X_train, y_train)

y_pred = model.predict(X_test)
```

---

## 📈 Model Evaluation

* Accuracy: **0.925 (92.5%)**

---

## 📌 Key Insights

* Age and salary significantly influence purchase behavior
* Logistic Regression effectively classifies customers
* Feature scaling improves model performance

---

## 🎯 Use Case

* Digital marketing → target potential buyers
* Companies → optimize ad campaigns
* Businesses → increase conversion rates

---

## 📌 Conclusion

Logistic Regression is effective for binary classification problems and can successfully predict customer purchasing behavior.

---

## 👨‍💻 Author

Ganesh Sharma
