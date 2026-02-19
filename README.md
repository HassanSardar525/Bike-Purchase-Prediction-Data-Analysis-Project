🚴 Bike Purchase Prediction – Data Analysis Project
📌 Project Overview

This project focuses on exploratory data analysis (EDA) and preprocessing of a Bike Purchase dataset containing demographic and socio-economic information of 1,000 customers.

The main objective is to analyze customer characteristics and understand patterns influencing whether a customer purchased a bike or not.

After data cleaning and preprocessing, the final dataset contains 919 records and 12 features, with all missing values handled and duplicates removed.

📊 Dataset Description
🔢 Shape

Original Shape: (1000, 13)

After Cleaning: (919, 12)

📋 Features
Column Name	Description
marital_status	Customer’s marital status
gender	Customer’s gender
income	Annual income (numeric)
children	Number of children
education	Education level
occupation	Job category
home_owner	Whether customer owns a house (Yes/No)
cars	Number of cars owned
commute_distance	Distance traveled to work
region	Geographic region
age	Customer’s age
purchased_bike	Target variable (Yes/No)
🧹 Data Cleaning & Preprocessing

✔ Removed duplicate rows
✔ Standardized column names (lowercase, snake_case)
✔ Handled missing values:

Numerical columns → Filled using median

Categorical columns → Filled using mode
✔ Resolved Pandas chained assignment warnings

Final dataset contains no missing values.

📈 Statistical Summary
🔹 Central Tendency & Spread

Income

Mean: 52,295

Median: 50,000

Std Dev: 27,133

Slight positive skew (0.53)

Children

Mean: 1.87

Median: 2

Std Dev: 1.61

Cars

Mean: 1.29

Median: 1

Age

Std Dev: 11.26

Moderate distribution spread

🔗 Correlation Insights
Variable 1	Variable 2	Correlation
Children	Age	0.54 (Strong positive)
Income	Children	0.26
Income	Cars	0.25
Cars	Age	0.23

🔎 Key Insight:
Older customers tend to have more children, and income moderately relates to number of cars owned.

📊 Categorical Insights (Mode Values)

Marital Status: Married

Gender: Male

Education: Bachelors

Occupation: Skilled Manual

Home Owner: Yes

Commute Distance: 0–1 Miles

Region: North America

Purchased Bike: No

Most customers in the dataset did not purchase a bike.

🎯 Objective

This dataset can be used for:

Classification Modeling (Logistic Regression, Decision Trees, Random Forest, etc.)

Customer segmentation

Marketing strategy optimization

Purchase behavior analysis

🛠️ Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

📌 Future Improvements

Apply Machine Learning models for bike purchase prediction

Feature engineering (income brackets, age groups, etc.)

Model evaluation using accuracy, precision, recall, F1-score

Deployment using Flask or FastAPI
