# Codtech-Task-4
 Insightful Sales Analytics with Python in Power BI
1. Project Overview

Title: Insightful Sales Analytics with Python in Power BI
Objective: Perform advanced data analysis and visualizations on sales data using Python scripts within Power BI to extract actionable insights.

Dataset: Sales dataset containing fields like:

OrderID, Product, Category, Sales, Profit, Discount, Region, Date

I can provide a ready-to-use CSV for this.

2. Power BI Setup with Python
Step 1: Enable Python in Power BI

Install Python (Anaconda recommended).

In Power BI Desktop:

File → Options and settings → Options → Python scripting

Set your Python home directory.

Step 2: Import Dataset

Home → Get Data → Excel/CSV

Load your sales dataset.

Step 3: Use Python Script

Home → Transform Data → Transform → Run Python Script

Example Python code for visualizations:

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# dataset is automatically loaded as 'dataset'
df = dataset

# 1. Sales vs Profit by Category
plt.figure(figsize=(8,6))
sns.scatterplot(x='Sales', y='Profit', hue='Category', data=df)
plt.title('Sales vs Profit by Category')
plt.show()

# 2. Total Sales by Region
sales_region = df.groupby('Region')['Sales'].sum().reset_index()
plt.figure(figsize=(8,6))
sns.barplot(x='Region', y='Sales', data=sales_region)
plt.title('Total Sales by Region')
plt.show()
3. Advanced Analysis Ideas

Top Products Analysis: Identify top-selling products by revenue.

Profit Margin Analysis: Highlight high vs low-profit categories.

Discount Effect: Analyze how discounts affect sales and profit.

Time Series Trends: Show sales trend over months using Python’s matplotlib or seaborn.

4. Visuals to Include in Power BI Report

Scatter plot: Sales vs Profit by Category

Bar chart: Total Sales by Region

Line chart: Monthly Sales Trend

Heatmap: Correlation between Sales, Profit, and Discount

You can use Python to generate these visuals and embed them directly in Power BI.

5. Deliverables for Submission

Power BI Report (.pbix) containing:

All Python-generated visualizations

Slicers/filters for interactivity (e.g., by Region, Category, Month)

README / Documentation including:

Project title and objective

Dataset description

Output
<img width="1373" height="771" alt="image" src="https://github.com/user-attachments/assets/e3199c6d-b612-4e31-8bca-76b8b6851ae4" />


Libraries used (pandas, matplotlib, seaborn)

Screenshots of key insights
