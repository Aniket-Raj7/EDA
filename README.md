# Exploratory Data Analysis (EDA) in Python
This repository demonstrates a step-by-step approach to performing Exploratory Data Analysis (EDA) using Python. The dataset used undergoes key EDA procedures, such as handling missing data, eliminating duplicates, and removing outliers using the Interquartile Range (IQR) method.

## Table of Contents
- Project Overview <br>
- Steps in the EDA Process <br>
- Handling Missing Values <br>
- Eliminating Duplicates <br>
- Detecting and Removing Outliers <br>
- Outlier Detection and Removal Using IQR <br>
- Formula for Outlier Detection <br> 
- Dependencies <br>
- Usage <br>
- Conclusion


## Project Overview
Exploratory Data Analysis (EDA) is an essential process in data science that involves summarizing the main characteristics of a dataset, often with visual methods. This project covers the key steps for performing EDA, focusing on:

Identifying and handling missing values.
Removing duplicate entries.
Detecting and eliminating outliers using the IQR method.
The aim is to clean the dataset for more reliable results in future analyses and model building.

## Steps in the EDA Process
**Step 1** <br> Handling Missing Values
In real-world datasets, missing values are common and need to be addressed to avoid bias in analysis. In this project, we:

- Identified columns with missing data.
Used appropriate techniques (e.g., removing rows, filling with median/mean) to handle these missing values.

**Step 2** <br> Eliminating Duplicates
Duplicate records can distort analysis by over-representing certain data points. We:

- Used the drop_duplicates() function to eliminate any duplicate rows in the dataset.

**Step 3** <br> Detecting and Removing Outliers
Outliers can skew the results of data analysis and predictive models. To address this, we 
- used the Interquartile Range (IQR) method to identify and remove outliers from the dataset. More details on this process are provided in the section below.
Outlier Detection and Removal Using IQR

Formula for Outlier Detection
The Interquartile Range (IQR) method is a statistical technique used to detect outliers in the dataset. It is based on quartiles, which divide the dataset into four equal parts.

## Here’s the process:

Q1: First quartile (25th percentile).<br>
Q3: Third quartile (75th percentile). <br>
IQR: The interquartile range is the difference between the third and first quartiles:
- IQR = 𝑄3 − 𝑄1
### Lower Bound:
  Lower Bound = 𝑄1 − 1.5 × IQR
### Upper Bound:
  Upper Bound = 𝑄3 + 1.5×IQR

- Data points that fall below the lower bound or above the upper bound are considered outliers. In this project, we applied this method to each numerical column of the dataset and removed rows containing these outliers.

## Dependencies
To replicate this EDA process, you need the following Python libraries:

- pandas for data manipulation and analysis
- numpy for numerical computations
- seaborn and matplotlib for visualizations


## Conclusion
This repository offers a simple yet effective framework for conducting Exploratory Data Analysis (EDA) in Python. Cleaning the data by eliminating missing values, duplicates, and outliers ensures a more accurate analysis, leading to better insights and more reliable predictive models.
Feel free to fork and modify the repository for your own EDA projects.
