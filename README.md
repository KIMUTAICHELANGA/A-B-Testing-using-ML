A/B Testing with Machine Learning Project
Overview
This project utilizes A/B testing combined with machine learning techniques to optimize user experiences. By comparing control and experiment groups, we aim to make data-driven decisions to enhance product features, marketing strategies, and overall user satisfaction.

Data
We have two datasets: control_data.csv and experiment_data.csv. Each contains information about pageviews, clicks, enrollments, and payments for different dates.

Number Summaries and Basic Investigations
Both datasets contain 37 entries with 5 columns: Date, Pageviews, Clicks, Enrollments, and Payments. There are missing values in Enrollments and Payments columns.

Data Wrangling
Combined control and experiment data.
Added row IDs and Day of Week features.
Removed missing data.
Added an Experiment column to denote control or experiment groups.
Removed Date and Payments columns.
Shuffled the data.
Model Building
Split the data into training and testing sets.
Converted Day of Week feature to numerical values.
Built models: Linear Regression, Decision Tree, XGBoost, and H2O AutoML.
Evaluated models using RMSE, R-squared, and MAE metrics.
Results
Linear Regression: RMSE=23.99, R2=0.051, MAE=19.59
Decision Tree: RMSE=26.85, R2=-0.189, MAE=21.78
XGBoost: RMSE=20.39, R2=0.314, MAE=17.77
H2O AutoML: RMSE=22.07, R2=0.196, MAE=20.27
Conclusion
XGBoost achieved the best performance with the lowest RMSE and highest R-squared. Further optimization and feature engineering can be explored for better results.
