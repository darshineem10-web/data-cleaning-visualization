# Thiranex-project-1
Data Cleaning and Visualization
This project focuses on cleaning, preprocessing, and visualizing a sample dataset using Python and Pandas.
The dataset contains information about employees, including their names, ages, salaries, joining dates, and departments. The project demonstrates basic data cleaning techniques and data visualization to prepare the dataset for further analysis.
Objectives

The main objectives of this project are:

- Inspect and understand the dataset
- Identify and handle missing values
- Remove duplicate records
- Detect and handle salary outliers
- Clean text data
- Convert date values into the appropriate format
- Encode categorical data
- Create visualizations to understand the cleaned data

- Technologies Used

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

- Dataset

The dataset contains employee-related information with the following columns:

Column| Description
Name| Name of the employee
Age| Age of the employee
Salary| Salary of the employee
Join_Date| Date the employee joined
Department| Department of the employee

The original dataset is included in the "data" folder.

Data Cleaning Process

The following data cleaning steps were performed:

1. Missing Values
   
   - Missing values in "Age" were filled using the median.
   - Missing values in "Salary" were filled using the mean.
   - Rows with missing "Join_Date" values were removed.

2. Text Cleaning
   
   - Extra spaces were removed from text-based columns.

3. Duplicate Removal
   
   - Duplicate records were identified and removed.

4. Outlier Handling
   
   - Salary outliers were identified using the Interquartile Range (IQR) method.
   - Records outside the defined IQR limits were removed.

5. Date Conversion
   
   - The "Join_Date" column was converted into a proper datetime format.

6. Categorical Encoding
   
   - The "Department" column was converted into numerical values using one-hot encoding.
  
   - Project Structure

data-cleaning-visualization/
│
├── README.md
├── Cleaning_Data.ipynb
│
├── data/
│   ├── sample_data.csv
│   └── cleaned_data.csv
│
└── visualizations/  

How to Run

1. Clone or download this repository.
2. Open "Cleaning_Data.ipynb" using Jupyter Notebook or JupyterLab.
3. Make sure the dataset is available inside the "data" folder.
4. Run the notebook cells in order.
5. The cleaned dataset will be generated as "cleaned_data.csv".

6. Conclusion

This project demonstrates the basic workflow of cleaning and preprocessing real-world-style data using Python. Missing values, duplicates, inconsistent text, outliers, dates, and categorical variables were handled before creating visualizations from the cleaned dataset.

This project helped build practical understanding of the data cleaning and visualization process in Data Science.
