Project Overview

This project explores the Superstore Sales dataset from Kaggle. The goal is to perform data cleaning, exploratory data analysis (EDA), and customer analysis, focusing on:

Sales trends over time

Profit and margin analysis

Product, category, and regional performance

Top customers using ABC analysis

Correlation between key variables

This analysis helps identify high-performing products, regions, and customers, as well as opportunities for improving profit margins.

2. Dataset

Source: Kaggle – Sample – Superstore

Number of rows: 9,994

Number of columns: 21

Key columns used in analysis:

Order Date, Segment, Region, Category, Sub-Category, Product Name, Sales, Profit, Profit Margin

3. Libraries Used
   
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from google.colab import files

5. Exploratory Data Analysis (EDA)
5.1 Sales Trends

Line chart showing total sales over time

Monthly sales trend by extracting month from Order Date

5.2 Category and Regional Analysis

Sales and Profit by Category (bar charts)

Sales and Profit by Region (horizontal bar charts)

Top 10 products by Sales and Profit

5.3 Customer Analysis

ABC analysis classifying customers into A, B, and C based on cumulative sales contribution

Table includes: Sales, Profit, Profit Margin, Cumulative %, ABC Category

5.4 Correlation Analysis

One-hot encoded categorical columns

The correlation heatmap shows relationship of Sales, Profit, and Profit Margin with Segment, Region, Category, and Sub-Category


6. Key Insights

1- The Dataset was already clean, and I searched for and found nothing wrong. I looked at using describe, info, and duplicated functions
2- With graphical analysis, I found that besides the sales being well distributed in the categories, technology was the most profitable representation, and the most outliers of high sales.
3- Sales and Profit across the regions are very correlated.
4-  Canon imageClass 2200 advanced Copier is the most sold and profitable product of the company, the rest and more evenly distributed. 
5- Going to the ABC curve, some problems were found, the best client has a negative profit, and some other clients to, which need to be addressed. 
6 - Analysing the correlation between the key columns with sales, profit, and profit margin, the most notable were: correlation of sub-category copiers with sales and profit, sub-category papel is negative with sales but positive in margin, the central region has negative correlation with margin, but the west is positive. 
