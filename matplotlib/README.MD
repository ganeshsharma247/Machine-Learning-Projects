# Iris Dataset Exploratory Data Analysis (EDA) 🌸📊

## 📌 Project Objective

The objective of this project is to perform Exploratory Data Analysis (EDA) on the Iris dataset to understand feature distributions, class relationships, and species separation using data visualization techniques.

---

## 📊 Dataset Information

* Source: Scikit-learn (Iris Dataset)
* Total Samples: 150
* Total Features: 4 numerical features

### Features:

* Sepal Length (cm)
* Sepal Width (cm)
* Petal Length (cm)
* Petal Width (cm)

### Target Classes:

* Setosa
* Versicolor
* Virginica

---

## 🎯 Project Type

* Exploratory Data Analysis (EDA)
* Data Visualization

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🚀 Project Workflow

1. Loaded Iris dataset using Scikit-learn
2. Converted dataset into a Pandas DataFrame
3. Added target labels and species names
4. Displayed:

   * First 5 records
   * Descriptive statistics
   * Class distribution
5. Created visualizations:

   * Class distribution bar chart
   * Histograms for feature distributions
   * Pair plot for feature relationships
   * Scatter plot for petal dimensions

---

## 💻 Code Snippet

```python id="irisx01"
sns.countplot(x='species', data=df)

sns.pairplot(df, hue='species', corner=True)

sns.scatterplot(
    x='petal length (cm)',
    y='petal width (cm)',
    hue='species',
    data=df
)
```

---

## 📈 Visualizations Performed

### 1. Class Distribution Bar Chart

* Shows the number of samples in each Iris species

### 2. Feature Histograms

* Displays the distribution of numerical features
* Helps identify spread, skewness, and outliers

### 3. Pair Plot

* Visualizes relationships between feature pairs
* Helps observe class separation

### 4. Scatter Plot

* Shows petal length vs petal width by species
* Clearly separates different flower species

---

## 📌 Key Insights

* Setosa species is clearly separable from others
* Petal features provide better class separation than sepal features
* Feature distributions vary significantly across species

---

## 🎯 Use Cases

* Beginner-friendly EDA project
* Understanding visualization techniques
* Dataset exploration before machine learning

---

## 📌 Conclusion

EDA and visualization techniques help understand data structure, feature relationships, and class separability before applying machine learning models.

---

## 👨‍💻 Author

Ganesh Sharma
