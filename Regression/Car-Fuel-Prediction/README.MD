# Car Fuel Efficiency Prediction using Linear Regression 🚗📊

## 📌 Project Objective

The objective of this project is to predict car mileage (MPG) based on engine size using a Machine Learning model

---

## 📊 Dataset Information

* The dataset contains:

  * **Engine_Size** → Size of the car engine
  * **MPG** → Fuel efficiency (miles per gallon)


## ⚙️ Algorithm Used

* Linear Regression

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

---

## 🚀 Project Workflow

1. Created dataset using Pandas
2. Defined input (X) and output (y)
3. Trained Linear Regression model
4. Predicted MPG for new engine size
5. Visualized results using graph

---

## 💻 Code Snippet

```python id="k1z0zq"
model = LinearRegression()
model.fit(X, y)

pred = model.predict([[200]])
print(pred)
```

---

## 📈 Output

Predicted MPG for engine size 200: **14.73**

---

## 📊 Visualization

* Blue dots represent actual data
* Red line represents regression line

---

## 📌 Conclusion

* As engine size increases, fuel efficiency (MPG) decreases
* Linear Regression successfully models this relationship

---

## 👨‍💻 Author

Ganesh Sharma
