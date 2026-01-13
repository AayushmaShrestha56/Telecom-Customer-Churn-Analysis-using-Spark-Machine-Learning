This assignment analyzes a telecom dataset using Spark for big data processing, performs exploratory data analysis and correlation analysis,
compares Spark operation performance, and builds an optimized Random Forest model to predict customer churn.

1. Dataset Loading & Environment Setup

You started by importing the required libraries such as Pandas and PySpark, and then:

Initialized a Spark Session to work with big data.

Loaded the telecom customer dataset into Pandas and Spark DataFrames.

Displayed sample rows to understand the structure of the data.
 Purpose:
To prepare the environment for big data analysis using both Pandas (small-scale inspection) and Spark (large-scale processing).

2. Exploratory Data Analysis (EDA)

You explored the dataset to understand customer behavior and data quality by:

Checking:

Dataset shape

Column data types

Missing values

Using:

df.info()

df.describe()

Frequency counts for categorical variables

Viewing distributions of:

Payment methods

Churn status

Service subscriptions

 Purpose:
To identify patterns, inconsistencies, and important features that influence customer churn.

3. Correlation Analysis

You included a correlation section where you:

Analyzed relationships between numerical features.

Observed how variables relate to customer churn.

Used graphs to visualize relationships (e.g., payment method vs churn).

 Purpose:
To understand which features are strongly related to churn and should be used in modeling.

4. Spark-Based Big Data Operations

You performed multiple Spark operations, including:

🔹 Aggregation

Calculated averages and summaries for numerical columns.

🔹 Customer Usage Analysis

Identified:

High data-usage customers

Frequently calling customers

🔹 Performance Measurement

Compared execution time and CPU usage of Spark operations.

 Purpose:
To demonstrate how Spark efficiently processes large telecom datasets and to compare performance across operations (important for your Assignment 2).

5. Hive / SQL-style Queries

You used Hive-like SQL queries on Spark DataFrames to:

Perform structured queries.

Simulate data warehousing operations.

Extract business insights using SQL logic.

Purpose:
To show integration of big data analytics with SQL-based querying, commonly used in telecom industries.

6. Data Cleaning & Preprocessing

In the DATA CLEANING section, you:

Checked inconsistent values (e.g., SeniorCitizen, TechSupport).

Handled missing or incorrect entries.

Ensured consistency between train and test datasets.

Prepared categorical variables for machine learning.

 Purpose:
To improve data quality, which directly impacts model accuracy.

7. Feature Engineering

Converted categorical features into dummy variables.

Selected relevant features for churn prediction.

👉 Purpose:
Machine learning models require numerical input, so this step prepares data for modeling.

8. Machine Learning – Random Forest

In the Random Forest section,

Trained a Random Forest classifier for churn prediction.

Used GridSearchCV to:

Tune hyperparameters

Improve model performance

Applied cross-validation for reliability.

👉 Purpose:
To build an accurate churn prediction model using an ensemble learning technique.

9. Model Evaluation

You evaluated the model using:

Accuracy and performance metrics.

Cross-validation results.

Comparison of parameter settings.

👉 Purpose:
To verify how well the model predicts customer churn and avoid overfitting.
