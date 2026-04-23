# Diabetes Progression Prediction using Regression Models 🧬📊

## 📌 Project Objective

The objective of this project is to predict disease progression in diabetes patients using multiple regression models.

---

## 📊 Dataset Information

* Source: Scikit-learn (Diabetes Dataset)
* Total Samples: 442
* Features: 10 baseline variables (age, BMI, blood pressure, etc.)

### Target:

* Disease progression measure (quantitative value)

---

## ⚙️ Algorithms Used

* Linear Regression
* Ridge Regression (L2 Regularization)
* Lasso Regression (L1 Regularization)

---

## 🛠️ Tools & Libraries

* Python
* Scikit-learn
* NumPy

---

## 🚀 Project Workflow

1. Loaded dataset using `load_diabetes()`
2. Split data into training (80%) and testing (20%)
3. Trained Linear Regression model
4. Trained Ridge Regression model
5. Trained Lasso Regression model
6. Predicted results on test data
7. Evaluated models using RMSE and R² score

---

## 💻 Code Snippet

```python id="xk3m7p"
lin_reg = LinearRegression()
lin_reg.fit(X_train, y_train)

ridge_reg = Ridge(alpha=1.0)
ridge_reg.fit(X_train, y_train)

lasso_reg = Lasso(alpha=0.1)
lasso_reg.fit(X_train, y_train)
```

---

## 📈 Model Evaluation

* RMSE (Root Mean Squared Error) → Lower is better
* R² Score → Higher is better

---

## 📌 Key Insights

* Linear Regression provides a baseline performance
* Ridge Regression helps reduce overfitting
* Lasso Regression performs feature selection by shrinking coefficients

---

## 📌 Conclusion

Regression models can effectively predict diabetes progression.
Regularization techniques improve model stability and interpretability.

---

## 👨‍💻 Author

Ganesh Sharma
