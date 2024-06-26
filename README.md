Summary of Exploratory Data Analysis (EDA) and Linear Regression on Air Quality Dataset
Exploratory Data Analysis (EDA):
Load the Data:

Loaded the dataset from an Excel file named "AirQualityUCI.xlsx".
Displayed the first few rows to understand the structure of the dataset.
Understand the Data Structure:

The dataset consists of 15 columns with various air quality measurements such as CO(GT), PT08.S1(CO), C6H6(GT), NOx(GT), and environmental factors like temperature and humidity.
Checked data types and missing values:
Most columns are of type float64.
The Date column is of type datetime64.
The Time column is of type object.
Data Cleaning:

Replaced -200 values with NaN to handle them as missing values.
Dropped the NMHC(GT) column due to a high percentage of missing values (90%).
Imputed missing values in other columns with the median.
Summary Statistics:

Generated summary statistics for the cleaned dataset, providing insights into the central tendency and variability of the data.
Linear Regression:
Variable Selection:

Selected PT08.S1(CO) as the independent variable (feature).
Selected CO(GT) as the dependent variable (target).
Data Preparation:

Split the data into training (80%) and testing (20%) sets using train_test_split.
Model Training:

Created a linear regression model using LinearRegression from scikit-learn.
Trained the model on the training data.
Model Prediction:

Used the trained model to predict CO(GT) values for the test data.
Model Evaluation:

Calculated Mean Squared Error (MSE) and R-squared (R²) to evaluate model performance:
MSE: Indicates the average squared difference between actual and predicted values.
R²: Indicates the proportion of variance in the dependent variable that is predictable from the independent variable.
Results Visualization:

Plotted the actual vs. predicted values to visualize the model's performance.
The scatter plot showed actual values, and the line plot showed predicted values.
