California Housing Price Prediction 🏡📊

📌 Problem Statement
Real-estate platforms, lenders, and urban planners need reliable estimates of house prices. Traditional methods fail to capture complex relationships between location, demographics, and housing features.
🎯 Project Objective
Build a supervised machine learning model to predict median house value (MedHouseVal) using multiple features from the California Housing dataset.

📊 Dataset Information
Source: Scikit-learn (California Housing Dataset)
Total Records: 20,640
Features:
MedInc → Median income
HouseAge → Age of houses
AveRooms → Average rooms
AveBedrms → Average bedrooms
Population → Total population
AveOccup → Average occupancy
Latitude → Location coordinate
Longitude → Location coordinate

Target:
MedHouseVal → Median house value (in $100,000s)
⚙️ Algorithms Used
Linear Regression
Ridge Regression (L2 Regularization)
Lasso Regression (L1 Regularization)
🛠️ Tools & Libraries
Python
Pandas
Scikit-learn

🚀 Project Workflow
Loaded dataset using fetch_california_housing()
Prepared features (X) and target (y)
Split dataset into training (80%) and testing (20%)
Trained Linear Regression model
Evaluated model using RMSE
Compared performance with Ridge and Lasso
💻 Code Snippet
lin_reg = LinearRegression()
lin_reg.fit(X_train, y_train)

y_pred = lin_reg.predict(X_test)
📈 Model Evaluation
Metric Used: RMSE (Root Mean Squared Error)
Lower RMSE indicates better model performance
📌 Key Insights
Linear Regression provides a baseline model
Ridge reduces overfitting when features are correlated
Lasso helps in feature selection by shrinking some coefficients to zero
🎯 Use Cases
Real-estate platforms → price estimation
Banks & lenders → risk analysis
Government agencies → urban planning

📌 Conclusion
Machine Learning models can effectively predict housing prices
Regularization techniques improve model generalization
Feature importance plays a key role in accurate predictions

👨‍💻 Author
Ganesh Sharma