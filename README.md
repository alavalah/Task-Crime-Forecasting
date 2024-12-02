# Task-Crime-Forecasting
Objective: The goal of this project is to develop an algorithm or model that accurately predicts crime hotspots in a specified jurisdiction using the provided Portland Police Bureau (PPB) Calls-for-Service (CFS) dataset.
Inspiration: This project is inspired by the National Institute of Justice’s Real-Time Crime Forecasting Challenge.
# Data Analysis and Preprocessing

# Loading the Dataset:

The dataset was loaded from a CSV file into a pandas DataFrame.
Initial exploration included displaying the first few rows, data types, and summary statistics.

# Handling Missing Data:

Rows with missing values were removed to ensure data quality.

# Feature Engineering:

The occ_date column was converted to datetime format.
New features were extracted: year, month, day, and day of the week.
Model Development

# Feature Selection:

Selected features: x_coordinate, y_coordinate, year, month, day, dayofweek.
Target variable: CATEGORY.

# Data Splitting:

The data was split into training (70%) and testing (30%) sets using train_test_split.

# Model Initialization:

A RandomForestClassifier was initialized with 100 decision trees (n_estimators=100) and a fixed random seed (random_state=42) for reproducibility.

# Model Training:

The model was trained on the training data.

# Making Predictions:

Predictions were made on the test data using the trained model.

# Evaluation Metrics

# Accuracy:

The accuracy of the model was calculated using accuracy_score.

# Confusion Matrix:

A confusion matrix was generated to visualize the performance of the model.

# Classification Report:

A classification report was generated to provide precision, recall, and F1-score for each class.
Visualization

# Crime Hotspots:

A scatter plot was created to visualize crime hotspots based on coordinates and categories.

# Grid Maps:
Provide visualizations of the forecasted crime hotspots.
Clearly indicate predicted high-risk areas- In a MAPS
Created grid maps and identified Strongly related features to burglary in the first week of 2013 in X and Y co-ordinates.

# Predicted Crime Hotspots:

A scatter plot of the predicted crime hotspots was created to visualize the model's predictions.
Prediction Accuracy Index (PAI) and Prediction Efficiency Index (PEI)

PAI Calculation:

PAI measures how well the model predicts crime hotspots.
It is calculated as the ratio of the number of crimes within the predicted hotspots to the total number of crimes.

PEI Calculation:

PEI evaluates the efficiency of the model by comparing the observed PAI to the optimal PAI.

# Report Generation

PDF Report:
A PDF report was generated summarizing the data exploration, model development, evaluation, and potential improvements.
Conclusion

Summary:

The developed model effectively predicts crime hotspots with a reasonable accuracy.
The visualizations and evaluation metrics provide insights into the model's performance.
Future Work:

Future improvements could include handling missing values using imputation techniques and exploring other machine learning algorithms for better performance.
