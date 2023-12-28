# User-Churn-Analysis-Waze

# Overview
The goal of this project was to decision tree based models like random forest and xgboost to predict whether or not a Waze user is retained or churned. This project utilized a synthetic dataset created in association with Waze. A data dictionary has been added to assist in the understanding to the dataset. The final xgboost model performed with 80.5% accuracy and 38.8% precision determining what features were most important in predicting which users will get churned or retained.

# Business Understanding
Waze’s free navigation app makes it easier for drivers around the world to get to where they want to go.Waze’s community of map editors, beta testers, translators, partners, and users helps make each drive better and safer. Waze partners with cities, transportation authorities, broadcasters, businesses, and first responders to help as many people as possible travel more efficiently and safely. The project is aimed to help prevent user churn on the Waze app. Developing a churn prediction model will help prevent churn, improve user retention and grow Waze's business.

# Data Understanding
The data consisted of 14999 unique users and 13 features. The features included information on number of drives made by users , number of times app was opened , total distance driven and so on. Approximately 18% of the dataset represents churned users and 82% represents retained users. In connection to this, few new features were engineered to represent if a user is a professional driver or not , distance driven per day and so on.

# Modeling and Evaluation
An XGBoost model comprising 300 decision trees was used to determine feature importance in which user will be churned or retained. The below plot shows that km_per_hour, percent_sessions_in_last_month and total_sessions_per_day are the 3 most important features to determine if the user will be churned or retained. The overall model performed with 80.5% accuracy and 38.8% precision.

![Waze -1](https://github.com/IamMayur95/User-Churn-Analysis-Waze/assets/67839699/030e7edc-2225-47b0-bc3b-ac308b4bdd2a)

Confusion matrix for the champion XGB model on test holdout data is as follows:

![Waze -2](https://github.com/IamMayur95/User-Churn-Analysis-Waze/assets/67839699/bb40fb95-941a-4dce-82bb-a0cb10c6c268)

# Conclusion
This modeling effort confirms that the current data is insufficient to consistently predict churn. It cannot be used to drive consequential business decisions. However, if the model is only being used to guide further exploratory efforts, then it can have value. 
