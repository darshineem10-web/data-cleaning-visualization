# Data Cleaning and Visualization

## Overview

This project demonstrates the process of cleaning, preprocessing, and visualizing an employee dataset using Python and Pandas.

The dataset contains employee information such as names, ages, salaries, joining dates, and departments. The goal is to identify and handle common data quality issues and prepare the dataset for further analysis.

## Objectives

- Understand and inspect the dataset
- Identify and handle missing values
- Remove duplicate records
- Detect and handle salary outliers
- Clean text data
- Convert date values into the appropriate format
- Encode categorical variables
- Create visualizations to understand the cleaned data

## Technologies Used

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

## Dataset

The dataset contains employee-related information with the following columns:

- Name
- Age
- Salary
- Join_Date
- Department

The original dataset contains missing values and potential salary outliers, which are handled during the cleaning process.

## Data Cleaning Process

The following steps were performed:

1. **Load the Dataset**
   - Loaded the CSV dataset using Pandas.

2. **Identify Missing Values**
   - Checked each column for missing values.

3. **Handle Missing Values**
   - Filled missing Age values using the median.
   - Filled missing Salary values using the mean.
   - Removed records with missing Join_Date values.

4. **Remove Duplicate Records**
   - Checked for duplicate records and removed duplicates based on Name and Age.

5. **Handle Salary Outliers**
   - Used the Interquartile Range (IQR) method to identify and filter salary outliers.

6. **Convert Data Types**
   - Converted Join_Date values into datetime format.

7. **Encode Categorical Variables**
   - Converted Department categories into numerical variables using one-hot encoding.

8. **Save the Cleaned Dataset**
   - Saved the processed data as `cleaned_data.csv`.

## Data Visualization

Matplotlib was used to visualize the cleaned dataset.

The project includes:

- **Department Distribution Bar Chart**
- **Salary Distribution Histogram**
- **Age and Salary Line Plot**

These visualizations help in understanding the distribution of employees and salary-related patterns in the cleaned dataset.

## Project Structure

```text
data-cleaning-visualization/
│
├── README.md
├── Cleaning data.ipynb
├── sample_data.csv
└── cleaned_data.csv

## How to Run

Clone or download this repository.
Open Cleaning data.ipynb in Jupyter Notebook.
Make sure sample_data.csv is in the same folder as the notebook.
Run the notebook cells in order.
The cleaned dataset will be generated as cleaned_data.csv.
The visualizations will be displayed in the notebook.

## Conclusion
This project demonstrates a basic data cleaning and preprocessing workflow using Python, Pandas, and Matplotlib. The cleaned dataset is structured and prepared for further analysis and visualization.
