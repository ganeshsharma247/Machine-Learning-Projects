# Breast Cancer Detection using Logistic Regression 🩺📊

## 📌 Problem Statement

Breast cancer is one of the most common cancers among women. Early and accurate diagnosis can reduce unnecessary biopsies and improve survival rates.
This project builds a machine learning model to classify tumors as **malignant** or **benign**.


## 🎯 Project Objective

Develop a supervised classification model that predicts whether a tumor is malignant or benign based on 30 numerical features extracted from medical images.



## 📊 Dataset Information

* Source: Scikit-learn (Breast Cancer Wisconsin Dataset)

### Features:

* 30 numerical features (e.g., radius, texture, perimeter, area, smoothness, concavity, symmetry)

### Target:

* 0 → Malignant (Cancerous)
* 1 → Benign (Non-cancerous)



## 🎯 Problem Type

* Binary Classification



## ⚙️ Algorithm Used

* Logistic Regression



## 🛠️ Tools & Libraries

* Python
* Scikit-learn
* NumPy



## 🚀 Project Workflow

1. Loaded dataset using `load_breast_cancer()`
2. Extracted features (X) and target (y)
3. Split dataset using stratified sampling (80% train, 20% test)
4. Trained Logistic Regression model
5. Predicted results on test data
6. Evaluated model using:

   * Accuracy
   * Confusion Matrix
   * Precision, Recall, F1-score



## 💻 Code Snippet

```python id="bc1x9a"
model = LogisticRegression()
model.fit(X_train, y_train)

y_pred = model.predict(X_test)
```


## 📈 Model Evaluation

* Accuracy Score
* Confusion Matrix
* Classification Report


## 📌 Key Insights

* High recall (sensitivity) is critical for malignant cases
* False negatives (missed cancer cases) must be minimized
* Logistic Regression provides a strong baseline model


## ⚠️ Clinical Focus

* **Recall (Sensitivity) for malignant class is most important**
* Missing a cancer case (False Negative) is more dangerous than a false alarm


## 🎯 Use Cases

* Clinical decision support systems
* Cancer diagnosis assistance
* Healthcare analytics


## 📌 Conclusion

Machine Learning models can assist in early cancer detection.
Focusing on recall ensures fewer missed malignant cases, improving patient safety.

---

## 👨‍💻 Author

Ganesh Sharma
