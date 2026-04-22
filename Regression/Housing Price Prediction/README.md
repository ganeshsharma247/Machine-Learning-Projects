# California Housing Price Prediction 🏡📊

## 📌 Problem Statement

Real-estate platforms, lenders, and urban planners need reliable estimates of house prices.
Traditional methods fail to capture complex relationships between location, demographics, and housing features.

---

## 🎯 Project Objective

Build a supervised machine learning model to predict **median house value (MedHouseVal)** using multiple features from the California Housing dataset.

---

## 📊 Dataset Information

* Source: Scikit-learn (California Housing Dataset)
* Total Records: 20,640

### Features:

* MedInc → Median income
* HouseAge → Age of houses
* AveRooms → Average rooms
* AveBedrms → Average bedrooms
* Population → Total population
* AveOccup → Average occupancy
* Latitude → Location
* Longitude → Location

### Target:

* MedHouseVal → Median house value (in $100,000s)

---

## ⚙️ Algorithms Used

* Linear Regression
* Ridge Regression (L2)
* Lasso Regression (L1)

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* Scikit-learn

---

## 🚀 Project Workflow

1. Loaded dataset using `fetch_california_housing()`
2. Prepared features (X) and target (y)
3. Split data (80% train, 20% test)
4. Trained Linear Regression model
5. Evaluated model using RMSE
6. Compared with Ridge and Lasso

---

## 💻 Code Snippet

```python
lin_reg = LinearRegression()
lin_reg.fit(X_train, y_train)

y_pred = lin_reg.predict(X_test)
```

---

## 📈 Model Evaluation

* Metric: RMSE (Root Mean Squared Error)
* Lower RMSE = Better performance

---

## 📌 Key Insights

* Linear Regression → baseline
* Ridge → reduces overfitting
* Lasso → feature selection

---

## 🎯 Use Cases

* Real-estate platforms → price estimation
* Banks → risk analysis
* Government → urban planning

---

## 📌 Conclusion

Machine Learning models can effectively predict housing prices.
Regularization improves model performance and generalization.

---

## 👨‍💻 Author

Ganesh Sharma
