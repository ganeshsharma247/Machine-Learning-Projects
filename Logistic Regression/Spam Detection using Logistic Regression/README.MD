# Spam Detection using Logistic Regression 📩🚫

## 📌 Problem Statement

Email services need to automatically classify messages as:

* Spam (unwanted messages)
* Not Spam (normal messages)

Incorrect classification can lead to important emails being missed or spam reaching users.

---

## 🎯 Project Objective

Build a machine learning model that predicts whether an SMS/email is spam or not based on message content.

---

## 📊 Dataset Information

* Source: Kaggle (SMS Spam Collection Dataset)

### Columns:

* label → spam / ham
* message → SMS text

### Target Encoding:

* 0 → Not Spam (ham)
* 1 → Spam

---

## 🎯 Problem Type

* Binary Classification
* Text Classification (NLP)

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
2. Selected relevant columns (label, message)
3. Converted labels (ham/spam → 0/1)
4. Converted text into numerical features using CountVectorizer
5. Split dataset into training (80%) and testing (20%)
6. Trained Logistic Regression model
7. Predicted results on test data
8. Evaluated model using:

   * Accuracy
   * Confusion Matrix
   * Precision, Recall, F1-score

---

## 💻 Code Snippet

```python id="sp1x9a"
vectorizer = CountVectorizer()
X = vectorizer.fit_transform(data['message'])

model = LogisticRegression()
model.fit(X_train, y_train)
```

---

## 📈 Model Evaluation

### Accuracy

* **0.977 (97.7%)**

### Confusion Matrix

```id="spcm01"
[[964   1]
 [ 24 126]]
```

### Metrics

* Precision: **0.99**
* Recall: **0.84**
* F1 Score: **0.91**

---

## 📌 Key Insights

* Model has very high precision → very few normal messages marked as spam
* Recall is slightly lower → some spam messages are missed
* F1 score shows good balance between precision and recall

---

## ⚠️ Important Metric Insight

* **Precision** → important to avoid marking normal emails as spam
* **Recall** → important to catch all spam messages
* Trade-off exists between both

---

## 🎯 Use Cases

* Email spam filters
* SMS filtering systems
* Fraud detection systems

---

## 📌 Conclusion

Logistic Regression combined with text vectorization effectively classifies spam messages.
Balancing precision and recall is crucial for optimal performance.

---

## 👨‍💻 Author

Ganesh Sharma
