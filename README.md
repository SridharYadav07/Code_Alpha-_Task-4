# Code_Alpha-_Task-4

Data Import and Exploration:
The necessary libraries for data manipulation, machine learning, and visualization are imported.
The dataset is loaded and checked for the top 5 rows, columns, data types, and missing values.

Data Preprocessing:
Handling Missing Values: Numerical columns are imputed using the mean of the respective column.
Categorical columns are imputed using the most frequent value of the respective column.

Label Encoding:
Binary categorical columns such as sex, fbs, and exang are label encoded into 0 and 1.

One Hot Encoding:
Columns with more than two categories are one hot encoded to create binary columns for each category.
The id, num, and dataset columns are dropped, and the target variable is separated from the features.

Data Splitting and Scaling:
The data is split into training and testing sets (80% training, 20% testing)
Feature scaling is applied using standardscaler to standardize the feature values so that they have a mean of 0 and a standard deviataion of 1.

Model Training and Evaluation:
A Random Forest classifier is trained on the training set.
Predictions are made on the test set, and the accuracy of the model is calcualted.
The classification report is printed, which includes metrics like precision, recall, f1-score and support.
A confusion matrix is generated to show the true vs predicted values. The confusion matrix is visualized using a heatmap for easier interpretaion.
