# Mobile Price Classification using Decision Tree and GridSearchCV 📱📊

## 📌 Problem Statement

Smartphone manufacturers and retailers need a way to estimate the price category of a mobile phone based on its hardware specifications. Predicting the correct price range helps businesses with pricing strategies and market positioning.

---

## 🎯 Project Objective

Build a machine learning model that predicts the price range of a mobile phone using its technical specifications.

The target variable contains four categories:

* 0 → Low Cost
* 1 → Medium Cost
* 2 → High Cost
* 3 → Very High Cost

---

## 📊 Dataset Information

* Source: Kaggle (Mobile Price Classification Dataset)
* Total Records: 2000 Mobile Phones
* Features: 20 Hardware Specifications

### Example Features

* Battery Power
* RAM
* Internal Memory
* Mobile Weight
* Screen Height
* Screen Width
* Clock Speed
* Pixel Resolution
* Number of Cores
* Camera Specifications
* Touch Screen Support
* 4G Availability

### Target

* price_range

---

## 🎯 Problem Type

* Multi-Class Classification

---

## ⚙️ Algorithm Used

### Decision Tree Classifier

Hyperparameter tuning performed using:

* GridSearchCV
* 5-Fold Cross Validation

Optimization Metric:

* F1 Macro Score

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

---

## 🚀 Project Workflow

1. Loaded mobile price dataset
2. Performed data inspection
3. Checked for missing values
4. Split dataset into training and testing sets
5. Applied GridSearchCV for hyperparameter tuning
6. Trained optimized Decision Tree model
7. Generated predictions on test data
8. Evaluated model performance
9. Analyzed feature importance
10. Visualized Decision Tree structure

---

## 💻 Code Snippet

```python
grid = GridSearchCV(
    DecisionTreeClassifier(random_state=42),
    param_grid=param_grid,
    cv=5,
    scoring='f1_macro',
    n_jobs=-1
)

grid.fit(x_train, y_train)
```

---

## 📈 Model Evaluation

Evaluation Metrics:

* Accuracy Score
* Classification Report
* Confusion Matrix
* F1 Macro Score

---

## 🔍 Hyperparameter Tuning

The following parameters were optimized:

* criterion
* max_depth
* min_samples_split
* min_samples_leaf
* max_features

GridSearchCV selected the best combination based on cross-validation performance.

---

## 📊 Feature Importance Analysis

The model identifies the most important features affecting mobile price prediction.

Examples:

* RAM
* Battery Power
* Pixel Resolution
* Internal Memory

Feature importance visualization was generated to understand which specifications influence pricing the most.

---

## 🌳 Decision Tree Visualization

The complete Decision Tree structure was visualized using:

* plot_tree()
* Feature Names
* Class Labels
* Colored Decision Nodes

This helps explain how the model makes decisions.

---

## 🎯 Business Use Cases

* Smartphone Pricing Strategy
* Product Market Analysis
* E-commerce Product Categorization
* Mobile Device Recommendation Systems

---

## 📌 Key Insights

* Hardware specifications strongly influence price range.
* RAM and battery power are among the most important predictors.
* Hyperparameter tuning significantly improves model performance.
* Decision Trees provide interpretable predictions.

---

## 📌 Conclusion

Decision Tree Classification combined with GridSearchCV successfully predicts mobile phone price categories. Feature importance analysis and tree visualization provide transparency into the model's decision-making process.

---

## 👨‍💻 Author

Ganesh Sharma
