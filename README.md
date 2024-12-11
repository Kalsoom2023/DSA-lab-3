# DSA-lab-3Lab 3: Data Analysis and Visualization

Overview

In this lab, we focus on data analysis and visualization using Python libraries such as Matplotlib and Pandas. You will work with CSV files to explore, manipulate, and visualize datasets, gaining insights through graphical representations.

Objectives

Understand and use Pandas for data manipulation and analysis.

Learn Matplotlib basics to create various types of visualizations.

Handle CSV files for reading and writing data.

Explore datasets and generate meaningful plots.

Requirements

Before starting this lab, ensure you have the following installed:

Python 3.x

Pandas

Matplotlib

Install the required libraries using pip if not already installed:

pip install pandas matplotlib

Tasks

1. Reading and Exploring CSV Data

Use pandas.read_csv() to load data from a CSV file.

Understand the structure of the dataset using functions like:

df.head() - View the first few rows.

df.info() - Get an overview of the dataset.

df.describe() - Get statistical summaries.

2. Data Manipulation

Perform common operations such as:

Filtering rows based on conditions.

Selecting specific columns.

Handling missing data using fillna() or dropna().

3. Data Visualization with Matplotlib

Create visualizations to analyze data trends and distributions:

Line Charts:

Use plt.plot() for continuous data.

Example: Plotting sales data over time.

Bar Charts:

Use plt.bar() for categorical comparisons.

Example: Visualizing population by region.

Scatter Plots:

Use plt.scatter() for relationships between two variables.

Example: Comparing height vs. weight.

Pie Charts:

Use plt.pie() to represent proportions.

Example: Market share distribution.

4. Writing CSV Data

Export manipulated data back to a CSV file using df.to_csv().

Ensure proper handling of file paths and delimiters.

Example Code

Here is a sample workflow:

import pandas as pd
import matplotlib.pyplot as plt

# Read CSV file
data = pd.read_csv('example.csv')

# Display dataset information
print(data.head())
print(data.info())

# Data manipulation: Filter data
filtered_data = data[data['column_name'] > 50]

# Visualization: Line chart
plt.plot(data['date'], data['value'])
plt.title('Value Over Time')
plt.xlabel('Date')
plt.ylabel('Value')
plt.show()

# Save filtered data to a new CSV file
filtered_data.to_csv('filtered_data.csv', index=False)

Deliverables

A Python script containing:

Data loading and manipulation.

Visualizations (at least 2 different types).

A summary of your findings based on the visualizations.

Learning Outcomes

By completing this lab, you will:

Be proficient in handling and analyzing datasets using Pandas.

Develop the ability to visualize data effectively using Matplotlib.

Gain experience in CSV file operations for real-world data scenarios.

Notes

Ensure your CSV files are well-formatted before analysis.

Experiment with different types of plots to find the most effective way to represent your data.
