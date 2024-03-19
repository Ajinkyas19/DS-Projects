
Laptop Price Predictor : Machine Learning Model

Overview
This document overviews the development of a machine learning model for predicting laptop prices using a dataset obtained from kaggle. The goal is to create an accurate and efficient model to analyze different components of laptop and predict the prices.

Data Loading and Exploration
1.	Data Loading
•	Loaded the dataset using Pandas function  read_csv from a CSV file.

2.	Initial Data Exploration
•	Examined the first 20 rows of the dataset to understand its structure.
•	Analyzed dataset features using info and describe function.

Data Cleaning and Preprocessing
3.	Data Cleaning
•	Checked data for missing values and outliers.
•	Corrected data types of 'Inches', 'Weight', and 'Price' from float to int.
•	Standardized the 'Ram' values and removed 'GB' units.
•	Processed 'ScreenResolution' values for better clarity.
•	Handled 'Memory' column to extract information about SSD, HDD, and Flash storage.


4.	Feature Engineering
•	Created new features 'ssd', 'hdd', and 'Flash or eMMc' based on 'Memory' information.
•	Engineered ‘cpuname’  to categorize CPU brands.

5.	Data Analysis
•	Explored the dataset, understanding the distribution of laptop features.
•	Checked the value counts for 'CompanyName', 'TypeOfLaptop', 'Ram', 'Gpu', 

6.	Data Visualization
•	Visualized relationships between key features and 'Price' using Matplotlib and Seaborn.

7.	Data Drop
•	Removed 'Memory' and 'Cpu' columns, which were no longer needed after feature engineering.

Data Splitting and Model Building
8.	Train-Test Split
•	Split the dataset into training and testing sets in 80:20 ratio using sklearn's train_test_split.

9.	Model Selection
•	Considered different regression models: Linear Regression and Decision Tree.

10.	Column Transformation
•	Used ColumnTransformer for one-hot encoding categorical columns.

11. Model Training
•	Trained a Linear Regression model as an initial algorithm along with Decision Tree Regressor.

12. Model Evaluation
•	Evaluated the model using R2 Score and Mean Absolute Error.

Conclusion
This machine learning model, implemented through a process of data preprocessing and model training, aims to accurately predict laptop prices, providing a valuable tool for users in the laptop market.

