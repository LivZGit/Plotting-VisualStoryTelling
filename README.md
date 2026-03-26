Question Title
Visualizing Sales and Distribution Data Using Matplotlib and Seaborn

Problem Statement
You are a data analyst presenting quarterly business insights to your team. Instead of sharing raw tables, your manager has asked you to create clear, well-labelled visualizations that tell a story about sales performance, score distributions, and product comparisons. You will generate synthetic data programmatically and produce four plots covering the chart types introduced in this session.

Data
Generate the dataset directly in your notebook using the code below — no external files required.

import pandas as pd
import numpy as np

np.random.seed(42)

months = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
          'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
sales = [12000, 15000, 13500, 17000, 16000, 19000,
         18500, 21000, 20000, 22500, 24000, 26000]

subjects = ['Math', 'Science', 'English', 'History', 'Art']
scores   = [78, 85, 72, 90, 65]

study_hours = np.random.uniform(1, 10, 100)
exam_scores = study_hours * 8 + np.random.normal(0, 5, 100)

product_sales = np.random.normal(loc=50, scale=10, size=200)

Tasks

Task 1 — Line Plot: Monthly Sales Trend
Using matplotlib, plot monthly sales over the 12-month period. Use months on the x-axis and sales on the y-axis. Customize the line color, add markers, and include a title and axis labels.

Task 2 — Bar Plot: Subject Score Comparison
Using matplotlib, create a bar plot comparing scores across five subjects. Add a title and axis labels. Make sure each bar is clearly readable.

Task 3 — Scatter Plot: Study Hours vs Exam Score
Using seaborn, create a scatter plot with study_hours on the x-axis and exam_scores on the y-axis. Add a title and axis labels.

Task 4 — Box Plot: Product Sales Distribution
Using seaborn, create a box plot for product_sales to visualize its distribution, median, and any outliers. Add a title and axis label.
