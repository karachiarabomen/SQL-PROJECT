# Orion Data Systems – Workforce Analytics Report(Jan - Oct 2026)


![SQL-header1](SQL-header1.png) 


## Executive Summary

This project analysed employee and workforce data for Orion Data Systems using SQL in MySQL Workbench. The analysis focused on workforce distribution, salary patterns, employee rankings, departmental leadership, job roles, and workforce gaps.

The results revealed that the workforce is concentrated in a few departments, with Shipping and Sales accounting for the largest employee groups. Salary analysis showed that 49 employees fall within the low salary band, 43 within the medium band, and 15 within the high salary band. The analysis also identified the highest-paying job roles, departments with the lowest average salaries, and countries with the highest total salary costs.

These findings provide useful insights into workforce structure, compensation distribution, and areas that may require further HR review.

.

The analysis covers ten business questions using SQL queries, including aggregate functions, joins, subqueries, Common Table Expressions (CTEs), and window functions.

## Business Context

Understanding workforce structure and salary distribution is important for effective human resource management. Organisations need to know how employees are distributed across departments, how compensation differs across roles, and whether staffing levels are balanced.

Orion Data Systems required a workforce analysis to examine employee distribution, salary patterns, departmental performance, and job-role compensation.

SQL was used to query, group, filter, rank, and aggregate the employee data to answer relevant workforce and business questions.


## Objectives

### The analysis aims to answer the following key business questions:

The objectives of this analysis were to:

- Examine employee distribution across departments.
- Compare salary levels across departments.
- Classify employees into salary bands.
- Identify departments with the lowest average salaries.
- Identify employees earning above the overall average salary.
- Analyse department leadership and employee counts.
- Identify job titles with average salaries above 12,000.
- Rank employees by salary within their departments.
- Compare total salary costs across countries.
- Identify job roles without assigned employees.



## Data Overview

The project uses four relational datasets representing the company's workforce and organisational structure.

### Database Structure

The four tables are connected through relevant identifiers, including employee IDs, department IDs, job IDs, and country IDs.

Database Schema: capstone 

Data Source: Supplied project datasets in CSV format.

The datasets contain structured employee and organisational information used to perform workforce analysis.

## Key Findings

## screnshots 

### The analysis investigates the following areas:

- Departments with the highest and lowest employee headcounts.
- Departments with the highest and lowest average salaries.
- Distribution of employees across low, medium, and high salary bands.
- Employees earning above the company-wide average salary.
- Job roles with average salaries above 12,000.
- Job roles without assigned employees.
- Employee salary rankings within departments.
- Total salary expenditure across countries.


## Data Cleaning and Transformation

MySQL was used to organise and analyse the supplied datasets.

### The preparation and analysis process included:

- Creating a dedicated database schema named "capstone".
- Working with four related workforce tables.
- Using table relationships and identifiers to connect employee, department, job, and country information.
- Handling NULL values when identifying job roles without assigned employees.
- Applying aggregate functions to calculate employee counts, average salaries, and total salary expenditure.
- Using CASE statements to classify employees into salary categories.
- Using CTEs and window functions to structure more advanced analysis.

## Detailed Findings & Analysis

### Workforce Distribution

Used COUNT, GROUP BY, and ORDER BY to calculate employee headcount across departments and identify departments with the largest workforce.

### Salary Comparison

Applied AVG and GROUP BY to calculate average employee salaries by department and identify salary differences across departments.

 ### Employee Salary Classification

Used CASE statements to classify employees into three salary categories:

- Low: Below 5,000
- Medium: 5,000–10,000
- High: Above 10,000

The analysis provides an overview of employee distribution across the salary bands.

### Country-Level Department Analysis

Used JOIN and COUNT to examine the number of departments operating in each country.

### Workforce Gaps

Applied RIGHT JOIN and NULL filtering to identify job roles in the jobs table that currently have no employees assigned.

### High Earners Analysis

Used a subquery and AVG function to identify employees whose salaries exceed the overall company average.

### Department Leadership Analysis

Applied INNER JOIN, GROUP BY, and COUNT to connect departments with their managers and calculate departmental employee headcount.

### Job Role Salary Analysis

Used a Common Table Expression (CTE), AVG, and HAVING to calculate average salaries by job title and identify roles with average salaries above 12,000.

### Employee Salary Ranking

Applied the ROW_NUMBER() window function with PARTITION BY and ORDER BY to rank employees by salary within their respective departments.

### Salary Expenditure by Country

Used JOIN, SUM, GROUP BY, and ORDER BY to calculate and compare total employee salary costs across countries.

## Recommendations

Based on the analysis, the following areas should be considered by the HR and Strategy team:

- Workforce Planning: Review departmental headcount to identify potential staffing imbalances.
- Compensation Management: Evaluate salary differences across departments and job roles to support fair and consistent compensation practices.
- Talent Allocation: Review job roles without assigned employees to determine whether recruitment or restructuring is necessary.
- Budget Management: Monitor salary expenditure across countries to improve workforce cost planning.
- Performance Monitoring: Use employee salary rankings and departmental salary analysis to support compensation reviews and workforce evaluation.

These recommendations should be validated against the actual analysis findings before implementation.

## Tools Used

MySQL: Used for querying, analysing, and extracting insights from the workforce database.

MySQL Workbench: Used as the database management and SQL development environment.

SQL Techniques: Used for data retrieval, aggregation, joins, subqueries, CTEs, CASE statements, and window functions.

## Conclusion

The Orion Data Systems Workforce Analytics project demonstrates how SQL can be used to investigate organisational workforce structures and answer important human resource business questions.

Through the analysis of employee records, departmental information, job roles, and country-level salary expenditure, the project applies SQL techniques to transform structured data into meaningful business insights.

The analysis provides a foundation for understanding workforce distribution, evaluating compensation structures, identifying potential staffing gaps, and supporting strategic HR decision-making.

## Project Information

**Project Title:** Orion Data Systems – Workforce Analytics

**Role:** Junior Data Analyst

**Industry:** Consulting & Technology

**Database:** MySQL

**Tools**: MySQL Workbench and SQL

**Project Category:** Human Resources Analytics
