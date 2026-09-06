📊 Data Analytics Portfolio — Transaction Analysis

<p align="center">
  <img src="https://img.shields.io/badge/Data%20Analytics-Professional-blue?style=for-the-badge" alt="Data Analytics">
  <img src="https://img.shields.io/badge/Python-Pandas-yellow?style=for-the-badge&logo=python" alt="Python Pandas">
  <img src="https://img.shields.io/badge/GitHub-Portfolio-black?style=for-the-badge&logo=github" alt="GitHub">
</p>

<h2 align="center">👨‍🏫 Md Safdar</h2>

<p align="center">
  <b>Senior Trainer — Data Analytics</b><br>
  Intensive Institute, New Delhi
</p>

<p align="center">
  <a href="mailto:safdar.ncpul@gmail.com">📧 Email</a> •
  <a href="tel:+919810845947">📞 +91-9810845947</a>
</p>

👋 About Me

I am Md Safdar, a Senior Trainer in Data Analytics at Intensive Institute, New Delhi.

I focus on practical, industry-oriented training in data analysis, Python, Pandas, data cleaning, visualization, and analytical problem solving.

This repository demonstrates a transaction-data analysis workflow using Python and Pandas, with an emphasis on data preparation and exploration.

📁 Project Overview

The supplied dataset contains 10,000 transaction records and 8 fields.

The dataset includes:

Field

Description

Transaction ID

Unique identifier for a transaction

Item

Item/product associated with the transaction

Quantity

Quantity purchased

Price Per Unit

Price of one unit

Total Spent

Total transaction amount

Payment Method

Payment method used

Location

Transaction location

Transaction Date

Date of the transaction

Source dataset: transaction records supplied for this GitHub project. The uploaded source contains the fields listed above. fileciteturn1file0L8-L8

🛠️ Technologies Used

🐍 Python

🐼 Pandas

📓 Jupyter Notebook

📈 Data Analysis & Visualization

🧹 Data Cleaning & Preprocessing

🗃️ JSON Data Handling

🐙 Git & GitHub

🔍 Suggested Data Analytics Workflow

1. Import Libraries

import pandas as pd

2. Load the Dataset

import json

with open("transaction_data.json", "r") as file:
    data = json.load(file)

df = pd.DataFrame(data)

3. Inspect the Dataset

df.head()
df.shape
df.info()
df.columns

4. Check Missing Values

df.isnull().sum()

5. Check Duplicate Records

df.duplicated().sum()

Remove duplicate rows:

df = df.drop_duplicates()

6. Find Unique Transaction IDs

df["Transaction ID"].unique().tolist()

7. Detect Invalid Values

To find rows containing values such as UNKNOWN or ERROR:

df[df.isin(["UNKNOWN", "ERROR"]).any(axis=1)]

To remove those rows:

df = df[~df.isin(["UNKNOWN", "ERROR"]).any(axis=1)]

📌 Example Pandas Operations

Filter Transactions

df[df["Quantity"] > 2]

Find Highest Transaction Amount

df["Total Spent"].max()

Calculate Average Spending

df["Total Spent"].mean()

Group by Item

df.groupby("Item")["Total Spent"].sum()

Group by Payment Method

df.groupby("Payment Method")["Total Spent"].sum()

📊 Potential Business Questions

This dataset can be used to answer questions such as:

Which items generate the highest revenue?

Which payment method is most frequently used?

Which locations generate the most sales?

What is the average transaction value?

Which products have the highest quantity sold?

How does revenue change over time?

What are the top-performing products?

Are there duplicate or invalid transactions?

What transaction patterns can be identified?

🎯 Learning Outcomes

After completing this project, learners can practice:

Data loading

Data inspection

Data cleaning

Missing-value analysis

Duplicate detection

Filtering and conditional selection

groupby() analysis

Aggregation functions

Data type handling

Basic exploratory data analysis

Preparing datasets for visualization

🧑‍🏫 Trainer Profile

Md Safdar

Senior Trainer — Data Analytics
Intensive Institute, New Delhi

Core Training Areas

Python • Pandas • Excel • SQL • Power BI • Data Cleaning • Data Visualization • Data Analytics

📧 Email: safdar.ncpul@gmail.com
📞 Contact: +91-9810845947

💼 GitHub Portfolio

This README is designed as a professional GitHub project introduction. You can place it in the root of your repository as:

README.md

Recommended project structure:

transaction-data-analysis/
│
├── README.md
├── data/
│   └── transaction_data.json
│
├── notebooks/
│   └── transaction_analysis.ipynb
│
├── scripts/
│   └── data_cleaning.py
│
├── reports/
│   └── analysis_report.pdf
│
└── visualizations/
    └── charts/

⭐ Project Highlights

Area

Skills Demonstrated

Data Loading

JSON, Pandas

Data Cleaning

Missing values, duplicates, invalid values

Data Exploration

head(), info(), describe()

Data Filtering

Boolean indexing

Aggregation

sum(), mean(), count(), groupby()

Business Analysis

Sales, products, locations, payments

Documentation

GitHub README

🚀 Future Enhancements

Add exploratory data analysis charts

Create an interactive Power BI dashboard

Add SQL queries for the same dataset

Build a complete Python data-cleaning pipeline

Add statistical analysis

Create an automated reporting workflow

Publish project insights and recommendations

📬 Contact

For Data Analytics Training, Python/Pandas Training, Excel, SQL, Power BI, or corporate training, connect with me:

Md Safdar
Senior Trainer — Data Analytics
Intensive Institute, New Delhi

📧 safdar.ncpul@gmail.com
📞 +91-9810845947

<p align="center">
  <b>📊 Learn • Analyze • Visualize • Decide</b><br>
  <i>Turning Data into Meaningful Insights</i>
</p>

<p align="center">
  ⭐ If you find this project useful, consider giving it a star!
</p>
