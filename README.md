# HR Employee Data Analysis Project

## Project Overview
The **HR Employee Data Analysis Project** uses Python to explore employee information, salary records, and attendance data. The goal is to organize the data, create visualizations, and identify useful patterns in workforce distribution, salary trends, and attendance records.

This is an educational project built with synthetic data. It is intended for Python practice and portfolio demonstrations, not for making real HR decisions.

## Dataset Information
The project contains three CSV files:

| File | Records | Description |
|---|---:|---|
| `employees.csv` | 2,000 | Employee details such as department, gender, city, date of birth, and employment type |
| `attendance.csv` | 256,000 | Weekday attendance records from January 1, 2026, through June 29, 2026 |
| `salary.csv` | 24,000 | Monthly salary records from October 2025 through September 2026 |

**Common join key:** `Employee_ID`

The values are fictional and do not represent real employees.

## Project Objectives
- Understand employee distribution across departments and cities.
- Explore gender and employment-type distribution.
- Analyze salary distribution and identify potential outliers.
- Track monthly salary expenditure.
- Review attendance status records.
- Examine relationships between salary components.
- Practice data cleaning, exploratory data analysis (EDA), and data visualization with Python.

## Tools and Libraries
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook or Google Colab

## Data Visualization Questions
The project includes the following chart questions:

1. **Department-wise Employee Distribution — Bar Chart**  
   How many employees are there in each department?

2. **Gender Distribution — Pie Chart**  
   How many male and female employees are there?

3. **Salary Distribution and Outliers — Box Plot**  
   What is the distribution of employee net salaries, and are there any potential salary outliers?

4. **City-wise Employee Distribution — Bar Chart**  
   How many employees work in each city?

5. **Monthly Salary Expenditure — Line Chart**  
   What is the monthly salary expenditure?

6. **Attendance Status — Count Plot**  
   How many attendance records are marked present, absent, or on leave?

7. **Correlation Between Salary Components — Heatmap**  
   What correlations exist between basic salary, allowances, bonuses, deductions, and net salary?

8. **Employee Salary Distribution — Histogram**  
   What is the distribution of employee salaries?

9. **Employment Type Distribution — Bar Chart**  
   How many employees work in each employment type?

## Data Analysis Workflow
1. Load the CSV files using Pandas.
2. Inspect column names, data types, and dataset sizes.
3. Check for missing values, duplicate records, and unusual values.
4. Convert date columns to datetime format where needed.
5. Summarize employee, salary, and attendance information.
6. Create charts using Matplotlib and Seaborn.
7. Write observations based on the actual results.
8. Summarize the findings and project limitations.

## How to Run the Project
1. Download or place `employees.csv`, `attendance.csv`, and `salary.csv` in your notebook's working folder.
2. Open Jupyter Notebook or Google Colab.
3. Install the required libraries if they are not already available:

   ```bash
   pip install pandas matplotlib seaborn
   ```

4. Import the libraries and load the CSV files:

   ```python
   import pandas as pd
   import matplotlib.pyplot as plt
   import seaborn as sns

   employees = pd.read_csv("employees.csv")
   attendance = pd.read_csv("attendance.csv")
   salary = pd.read_csv("salary.csv")
   ```

5. Run the data cleaning, analysis, and chart code for each question.

## Key Business Insights
The charts can help explore:
- Which departments and cities have the most employees.
- How employees are distributed by gender and employment type.
- How net salaries vary and whether potential outliers exist.
- How total net salary expenditure changes by month.
- How attendance records are distributed across attendance statuses.
- How salary components are related to one another.

These are analysis goals, not pre-confirmed findings. Final insights should be written only after reviewing the actual charts and calculated results.

## Conclusion
This project demonstrates how Python can be used to analyze HR datasets and communicate patterns through visualizations. Pandas supports data loading and analysis, while Matplotlib and Seaborn help present the results clearly. The project provides practice in data preparation, exploratory data analysis, and drawing evidence-based observations from employee, salary, and attendance records.

## Limitations
- The dataset is synthetic and fictional.
- Attendance data covers January 1, 2026, through June 29, 2026, while salary data covers October 2025 through September 2026.
- The number of salary records does not mean there are that many unique employees; employees can have records for multiple months.
- Attendance charts count attendance records unless the code explicitly calculates unique employees.
- Correlation indicates association, not cause and effect.
- Potential outliers should be checked before deciding whether they are errors.

## Author
Created as a Python data analysis project for learning and portfolio practice.
