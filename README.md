##  Employee Data Analysis Project
This project involves analyzing a dataset of employees using Excel and XLSTAT to understand various features and perform data preprocessing, visualization, and modeling.

# Project Structure
# Datasets: 
Contains the raw and processed datasets.
# Scripts:
Contains Excel and XLSTAT scripts for data processing and analysis.
# Documentation:
Contains detailed documentation and reports of the analysis.
# Step-by-Step Documentation
# 1. Understanding the Initial Dataset
We start by understanding the features of the employee dataset and performing initial preprocessing steps.

# 2. Formatting Dates and Calculating Age
Ensure that the bdate (birthdate) column is correctly formatted as a date.
Compute the age of each employee by finding the difference between today's date and the birthdate.
# 3. Transforming Education Years to Education Category
Convert the number of education years to education categories using conditional formulas.

# 4. Identifying and Removing Noise or Null Values
Use the filter option to check for null values in the dataset.
Remove rows with any null values to ensure the dataset is clean and ready for further analysis.
# 5. Creating Frequency Tables and Charts
Create a frequency table to show the count and proportion of individuals in each education category.
Use the frequency data to create bar charts for education levels and relative frequencies.
Create a Pareto chart combining the frequency data and cumulative frequency percentage.
# 6. Creating Pivot Tables
Based on Minority Status and Gender: Analyze the distribution of minority status across different genders, resulting in a bar chart that shows 170 male minority employees and 31 female minority employees.
Based on Job Categories: Analyze the distribution of employees across different job categories, resulting in a pie chart that shows Jobcat-1 with 316 employees, Jobcat-2 with 23 employees, and Jobcat-3 with 71 employees.
Based on Education Categories: Analyze the distribution of employees across different education categories, resulting in a pie chart that shows PhD (1), Masters (21), School (46), Bachelors (72), College (103), and High School (167).
# 7. Histogram Analysis
# Age:
Not normally distributed with details such as Max (95), Min (53), Skewness (0.93343652), QRT1 (58), QRT2/Median (62), QRT3 (75), IQR (17), Deviation (131.762112), and StdDev (11.4787679).
# Salary:
Not normally distributed with details such as Max (86,250), Min (16,200), Skewness (1.66214127), QRT1 (24,300), QRT2/Median (28,800), QRT3 (36,000), IQR (11,700), Deviation (201,184,288.7), and StdDev (14,183.94475).
# Starting Salary:
Not normally distributed with details such as Max (45,000), Min (9,750), Skewness (1.962550765), QRT1 (12,750), QRT2/Median (15,000), QRT3 (17,250), IQR (4,500), Deviation (40,545,368.28), and StdDev (6,367.524502).
# Previous Experience: 
Not normally distributed with details such as Max (432), Min (0), Skewness (1.45759502), QRT1 (19), QRT2/Median (52), QRT3 (81), IQR (62), Deviation (201,184,288.7), and StdDev (14,183.94475).
# 8. Boxplot Analysis
Boxplots are used to make decisions based on the IQR, QRT1, and QRT3.
Consider using the 99th percentile for more precise decision-making.
Note that QRT2 (the median) and the mean are equal.
# 9. Normality Test Results
The normality tests show that for all features, the p-value is less than 0.05, confirming that the data is not normally distributed. Normalizing and standardizing the data does not change the distribution.

# 10. Evaluation of Chi-Square and Gamma Distributions
The data does not follow Chi-square and Gamma distributions, as the p-value is less than 0.05, leading to the rejection of the null hypothesis.

# 11. Identification and Removal of Outliers Using Quantiles
Identify outliers using the 0.99 and 0.01 quantiles and remove extreme data points.

# 12. Correlation Matrix
Salary and Job Category: Significant correlation.
Salary and Minority Status: Biserial correlation coefficient (r) of -0.150 and a p-value of <0.0001, indicating a significant association.
Salary and Gender: Biserial correlation coefficient (r) of -0.445 and a p-value of <0.0001, indicating a significant association.
# 13. Modeling
Performed regression analysis to build a model using the variables norm-salary, norm-salbegin, and jobcat.

# Usage
Clone the repository.
Open the Excel files and follow the documentation steps for data preprocessing and analysis.
Use XLSTAT for advanced statistical analysis as detailed in the documentation.
# Requirements
Excel
XLSTAT
