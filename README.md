# Below is a Python script that creates a small dataset, analyzes it using basic statistical measures, and showcases familiarity with data analysis tools like Pandas and NumPy

import pandas as pd
import numpy as np

# Create a small dataset
data = {'Name': ['Alice', 'Bob', 'Charlie', 'David', 'Emma'],
        'Age': [25, 30, 35, 40, 45],
        'Salary': [50000, 60000, 70000, 80000, 90000]}
df = pd.DataFrame(data)

# Display the dataset
print("Dataset:")
print(df)
print()

# Calculate basic statistical measures
mean_age = np.mean(df['Age'])
mean_salary = np.mean(df['Salary'])
median_age = np.median(df['Age'])
median_salary = np.median(df['Salary'])
mode_name = df['Name'].mode()[0]
std_age = np.std(df['Age'])
std_salary = np.std(df['Salary'])
range_age = np.max(df['Age']) - np.min(df['Age'])
range_salary = np.max(df['Salary']) - np.min(df['Salary'])

# Display results
print("Basic Statistical Measures:")
print(f"Mean Age: {mean_age}")
print(f"Mean Salary: {mean_salary}")
print(f"Median Age: {median_age}")
print(f"Median Salary: {median_salary}")
print(f"Mode Name: {mode_name}")
print(f"Standard Deviation Age: {std_age}")
print(f"Standard Deviation Salary: {std_salary}")
print(f"Age Range: {range_age}")
print(f"Salary Range: {range_salary}")


# This script will output the dataset and the calculated basic statistical measures in a single run
