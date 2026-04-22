# Advertising Sales Prediction using Multiple Linear Regression 📊📺

## 📌 Project Objective

The objective of this project is to predict product sales based on advertising spend across different channels:

* TV Ads
* Radio Ads
* Newspaper Ads

---

## 📊 Dataset Information

* Source: Kaggle (Advertising Dataset)

### Features:

* TV → Advertising budget spent on TV
* Radio → Advertising budget spent on Radio
* Newspaper → Advertising budget spent on Newspaper

### Target:

* Sales → Product sales

---

## ⚙️ Algorithm Used

* Multiple Linear Regression

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* Scikit-learn

---

## 🚀 Project Workflow

1. Imported required libraries
2. Loaded dataset using Pandas
3. Selected features (TV, Radio, Newspaper)
4. Defined target variable (Sales)
5. Split dataset into training (80%) and testing (20%)
6. Trained Multiple Linear Regression model
7. Predicted sales on test data
8. Evaluated model using RMSE

---

## 💻 Code Snippet

```python id="r0m5lw"
model = LinearRegression()
model.fit(x_train, y_train)

y_pred = model.predict(x_test)
```

---

## 📈 Model Evaluation

* RMSE (Root Mean Squared Error): **1.705**

---

## 📌 Key Insights

* Advertising spend strongly impacts product sales
* TV and Radio ads have higher influence compared to Newspaper ads

---

## 📌 Conclusion

Multiple Linear Regression effectively models the relationship between advertising spend and sales.

---

## 👨‍💻 Author

Ganesh Sharma
