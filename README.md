# Orion Data Systems – Workforce Analytics Report(October 2026) 


## Executive Summary

This project analyses the workforce database of Orion Data Systems, a multinational consulting and technology firm operating across Europe, Asia, and the Americas.

Using MySQL, the analysis examines employee distribution, salary structures, departmental performance, job roles, and geographical salary expenditure.

The objective is to provide the HR and Strategy team with meaningful workforce insights that can support compensation analysis, workforce planning, and strategic decision-making.

The analysis covers ten business questions using SQL queries, including aggregate functions, joins, subqueries, Common Table Expressions (CTEs), and window functions.

## Business Context

Managing a multinational workforce requires accurate information about employee distribution, compensation, departmental structures, and job assignments.

Orion Data Systems needs a clearer understanding of how its workforce is distributed across departments and countries, how employee salaries compare, and whether existing job roles are adequately staffed.

The HR and Strategy team requires data-driven insights to evaluate workforce structures, identify potential staffing gaps, understand salary expenditure, and support effective human resource planning.

This analysis uses SQL to investigate these areas and provide insights that can support informed business decisions.

## Objectives

### The analysis aims to answer the following key business questions:

- How is the workforce distributed across departments, and which department has the highest employee headcount?
- What are the average salary differences across departments and job roles?
- How are employees distributed across different salary bands?
- Which employees earn above the company's overall average salary?
- Which job roles currently have no employees assigned?
- How are employee salary costs distributed across different countries?



## Data Overview

The project uses four relational datasets representing the company's workforce and organisational structure.

### Database Structure

The four tables are connected through relevant identifiers, including employee IDs, department IDs, job IDs, and country IDs.

Database Schema: capstone 

Data Source: Supplied project datasets in CSV format.

The datasets contain structured employee and organisational information used to perform workforce analysis.

## Key Findings

## screnshots 

The analysis investigates the following areas:

- Departments with the highest and lowest employee headcounts.
- Departments with the highest and lowest average salaries.
- Distribution of employees across low, medium, and high salary bands.
- Employees earning above the company-wide average salary.
- Job roles with average salaries above 12,000.
- Job roles without assigned employees.
- Employee salary rankings within departments.
- Total salary expenditure across countries.

Specific findings and numerical results will be added after reviewing the executed SQL query outputs.

6. Data Cleaning and Transformation

MySQL was used to organise and analyse the supplied datasets.

The preparation and analysis process included:

- Creating a dedicated database schema named "capstone".
- Working with four related workforce tables.
- Using table relationships and identifiers to connect employee, department, job, and country information.
- Handling NULL values when identifying job roles without assigned employees.
- Applying aggregate functions to calculate employee counts, average salaries, and total salary expenditure.
- Using CASE statements to classify employees into salary categories.
- Using CTEs and window functions to structure more advanced analysis.

## Detailed Findings & Analysis

7.1 Workforce Distribution

Used COUNT, GROUP BY, and ORDER BY to calculate employee headcount across departments and identify departments with the largest workforce.

7.2 Salary Comparison

Applied AVG and GROUP BY to calculate average employee salaries by department and identify salary differences across departments.

7.3 Employee Salary Classification

Used CASE statements to classify employees into three salary categories:

- Low: Below 5,000
- Medium: 5,000–10,000
- High: Above 10,000

The analysis provides an overview of employee distribution across the salary bands.

7.4 Country-Level Department Analysis

Used JOIN and COUNT to examine the number of departments operating in each country.

7.5 Workforce Gaps

Applied RIGHT JOIN and NULL filtering to identify job roles in the jobs table that currently have no employees assigned.

7.6 High Earners Analysis

Used a subquery and AVG function to identify employees whose salaries exceed the overall company average.

7.7 Department Leadership Analysis

Applied INNER JOIN, GROUP BY, and COUNT to connect departments with their managers and calculate departmental employee headcount.

7.8 Job Role Salary Analysis

Used a Common Table Expression (CTE), AVG, and HAVING to calculate average salaries by job title and identify roles with average salaries above 12,000.

7.9 Employee Salary Ranking

Applied the ROW_NUMBER() window function with PARTITION BY and ORDER BY to rank employees by salary within their respective departments.

7.10 Salary Expenditure by Country

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

11. Project Information

Project Title: Orion Data Systems – Workforce Analytics

Role: Junior Data Analyst

Industry: Consulting & Technology

Database: MySQL

Tools: MySQL Workbench and SQL

Project Category: Human Resources Analytics
