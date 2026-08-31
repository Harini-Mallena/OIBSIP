# Task 3 - Data Cleaning using Python

## About the Project

This project is about cleaning the Titanic dataset using Python.
I used Pandas and NumPy to find the problems in the dataset and
clean the data so that it can be used for further analysis.

## Tools Used

- Python
- Pandas
- NumPy
- Jupyter Notebook

## Dataset

I used the Titanic dataset which contains information about the
passengers.

Some of the important columns are:

- PassengerId
- Survived
- Pclass
- Name
- Sex
- Age
- SibSp
- Parch
- Ticket
- Fare
- Cabin
- Embarked

## What I Did in This Project

### 1. Data Quality Check

First, I checked the dataset to understand the data and find the
existing problems.

I checked:

- Null values
- Data types
- Duplicate rows
- Minimum and maximum values
- Possible value range anomalies

### 2. Missing Values

I checked the number and percentage of missing values in each column.

For handling missing values:

- Age → Filled missing values using the median
- Embarked → Filled missing values using the mode
- Cabin → Removed because it had a large number of missing values

### 3. Duplicate Rows

I checked the dataset for duplicate rows and removed exact duplicate
records if they were present.

### 4. Standardisation

I standardized the text and categorical columns.

I:

- Removed unnecessary spaces
- Standardized `Sex` values
- Standardized `Embarked` values

### 5. Outlier Detection

I used the IQR (Interquartile Range) method to find possible outliers
in the numerical columns.

I checked columns such as:

- Age
- SibSp
- Parch
- Fare

The detected outliers were reviewed instead of directly deleting them.
Since the values can represent actual passengers or valid ticket
fares, the potential outliers were retained.

### 6. Data Type Correction

I checked the data types again after cleaning.

`PassengerId` was treated as an identifier, while numerical and
categorical columns were kept in appropriate data types.

### 7. Before and After Comparison

I compared the dataset before and after cleaning to check:

- Null values
- Duplicate rows
- Number of rows
- Number of columns
- Data type accuracy

## Final Result

After cleaning, the dataset is ready for further analysis.

The cleaned dataset was saved as:

`titanic_cleaned.csv`

## Files

- `Task_3_Data_Cleaning.ipynb` - Jupyter Notebook containing the complete cleaning process
- `titanic_cleaned.csv` - Cleaned Titanic dataset
- `README.md` - Project description

## What I Learned

Through this task, I learned how to:

- Check data quality using Pandas
- Handle missing values
- Remove duplicate records
- Standardize categorical data
- Detect outliers using IQR
- Correct data types
- Compare data before and after cleaning
- Save a cleaned dataset as a CSV file
