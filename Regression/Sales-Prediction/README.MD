Advertising Sales Prediction using Multiple Linear Regression 📊📺

📌 Project Objective

The objective of this project is to predict product sales based on advertising spend across different channels:
TV Ads
Radio Ads
Newspaper Ads

📊 Dataset Information
Source: Kaggle (Advertising Dataset)
Features:
TV → Advertising budget spent on TV
Radio → Advertising budget spent on Radio
Newspaper → Advertising budget spent on Newspaper
T
arget:
Sales → Product sales
⚙️ Algorithm Used
Multiple Linear Regression

🛠️ Tools & Libraries
Python
Pandas
Scikit-learn

🚀 Project Workflow
Imported required libraries
Loaded dataset using Pandas
Selected features (TV, Radio, Newspaper)
Defined target variable (Sales)
Split dataset into training and testing sets
Trained Multiple Linear Regression model
Predicted sales on test data
Evaluated model using RMSE

💻 Code Snippet
model = LinearRegression()
model.fit(x_train, y_train)

y_pred = model.predict(x_test)

📈 Model Evaluation
RMSE (Root Mean Squared Error): 1.705
📌 Conclusion
Advertising spend has a strong impact on product sales
TV and Radio ads contribute more significantly compared to Newspaper ads
Multiple Linear Regression effectively models the relationship
👨‍💻 Author
Ganesh Sharma
