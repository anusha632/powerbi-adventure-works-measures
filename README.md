# Power BI – Adventure Works Measures

This project showcases my hands-on practice with measures in Power BI, using the Adventure Works dataset.
The focus is on creating calculations both with Quick Measures and by writing DAX expressions,
which are essential skills for data analysis and reporting in Power BI.

Project Overview
Tool used: Power BI Desktop
Dataset: Adventure Works
Main focus: Creating and formatting measures for sales analysis

# Measures Created

1. Running Total in Year
This measure was created using Power BI’s Quick Measure feature.
It calculates the cumulative (running) total of sales across each year,
which helps in understanding sales trends over time.

Based on:
Sales[Total Sales]
Date[Year]

Displays results as currency, formatted to two decimal places

2. Total Revenue
This measure was created by writing a custom DAX expression.
It calculates total revenue by multiplying the unit price of each product by the quantity sold,
and then summing the result across all rows.

Total Revenue =
SUMX (
    Sales,
    Sales[Unit Price] * Sales[Quantity]
)

The measure is formatted as currency with two decimal places for better readability and consistency.

# Outcome

By completing this exercise, I strengthened my understanding of:
- Using Quick Measures for common calculations
- Writing DAX measures using functions like SUMX
- Formatting measures correctly for financial reporting

This project demonstrates my ability to work with Power BI measures to support business-focused data analysis.



