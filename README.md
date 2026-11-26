# Orion Data Systems – Workforce Analytics Report(Jan - Nov 2026)


![SQL-header1](SQL-header1.png) 


## Executive Summary
This project analysed workforce data for Orion Data Systems using SQL in MySQL Workbench. The analysis focused on employee distribution, salary patterns, departmental leadership, job-role compensation, employee salary ranking, and country-level salary costs.
The findings showed that employee numbers were concentrated in a few departments, particularly Department 50 and Department 80. Salary-band analysis revealed that 49 employees fell within the low salary band, 43 within the medium salary band, and 15 within the high salary band.
The project also identified job titles with average salaries above 12,000, examined employees earning above the overall average salary, and compared total salary costs across countries.
The analysis demonstrates how SQL can be used to transform workforce data into meaningful insights that support human resource management and workforce planning.


## Business Context
- Workforce data provides organisations with important information about employee distribution, compensation, departmental structure, and staffing needs.
- Orion Data Systems required an analysis of its workforce to understand how employees were distributed across departments, how salaries differed, and how compensation and staffing patterns varied across job roles and countries.
SQL was used to retrieve, filter, group, rank, and aggregate the data to answer relevant business questions.

## Project Objectives

### The objectives of this analysis were to:
- Examine employee distribution across departments.
- Compare salary levels across departments.
- Classify employees into salary bands.
- Identify departments with the lowest average salaries.
- Identify employees earning above the overall average salary.
- Analyse department leadership and employee counts.
- Identify job titles with average salaries above 12,000.
- Rank employees by salary within their departments.
- Compare total salary costs across countries.
- Identify job records without matching employee records.


   ## Data Analysis and Key Findings
### Workforce Distribution
The workforce distribution analysis examined the number of employees in each department.

**The largest employee groups were:**
Department ID	Employee Count
50	                   45
80	                   34
100                    6
30	                    6
60	                    5
Department 50 had the highest employee count, followed by Department 80.


### Business Insight:
Employee concentration in these departments highlights their importance within the organisation. Management can use this information to review staffing levels and ensure that workforce allocation supports operational needs.

### Salary Band Analysis
Employees were classified into salary bands using a SQL CASE statement.
Salary Band	Number of Employees
Low	               49
Medium            	43
High	               15
The low salary band contained the largest number of employees, while the high salary band contained the fewest.

![salary_bond](usingcasestatement.png) 

**Business Insight:** The salary distribution provides an overview of compensation levels within the workforce. It can support further review of salary structures, job levels, and opportunities for employee progression.


4.3 Department Average Salary Analysis
The analysis identified the three departments with the lowest average salaries.
Department ID	Average Salary
50	3,475.56
30	4,150.00
10	4,400.00
Department 50 recorded the lowest average salary among the departments returned by the query.
Business Insight: Differences in departmental average salaries may reflect variations in job roles, employee seniority, or workforce composition. Further investigation can help management understand these differences.
4.4 High-Earning Employees
A subquery was used to identify employees earning more than the overall average salary.
Examples from the results included:
Employee	Salary
Steven King	24,000
Neena Kochhar	17,000
Lex De Haan	17,000
John Russell	14,000
Karen Partners	13,500
Business Insight: Identifying employees earning above the overall average provides a useful starting point for compensation comparisons and understanding salary distribution across the organisation.
4.5 Department Leadership Analysis
The department leadership query examined department names, manager names, and employee counts.
Department	Manager	Employee Count
Shipping	Michael Johnson	45
Sales	Sophia Martinez	34
Finance	David Jacobs	6
Purchasing	Rebecca Chen	6
IT	Cynthia Morrison	5
Executive	Anthony Rodriguez	3
Shipping and Sales had the largest employee counts among the departments displayed.
Business Insight: Department-level employee counts provide information about workforce structure and managerial responsibilities. This can support staffing reviews and resource allocation.
4.6 Job Role Salary Analysis
The job-role analysis identified job titles with average salaries greater than 12,000.
Job Title	Average Salary
President	24,000
Administration Vice President	17,000
Marketing Manager	13,000
Sales Manager	12,200
President had the highest average salary among the job titles returned.
Business Insight: The results show differences in average compensation across job roles and can support salary benchmarking and compensation planning.
4.7 Employee Salary Ranking
The employee ranking analysis uses the SQL ROW_NUMBER() window function to rank employees by salary within their departments.
The corrected query partitions employees by department and orders their salaries from highest to lowest. This assigns rank 1 to the highest-paid employee within each department.
Business Insight: Department-level salary ranking allows the organisation to compare employee compensation within individual departments. It can support internal salary reviews and workforce analysis.
4.8 Country-Level Workforce Analysis
The country-level workforce query examined the number of distinct departments represented in each country.
The results showed that Australia had 4 departments, while Belgium, Brazil, Canada, China, and Egypt each had 3 departments in the displayed results.
Business Insight: This analysis provides an overview of departmental presence across countries and can help management understand the organisation's geographical workforce structure.
4.9 Country-Level Salary Cost Analysis
The country salary cost query aggregated employee salaries by country and sorted the results from highest to lowest.
Country	Total Salary Cost
Switzerland	75,100
Italy	52,100
Israel	45,200
Argentina	43,600
China	42,400
Egypt	41,600
Brazil	38,000
Japan	33,600
Belgium	33,600
India	32,800
United States	31,600
Kuwait	25,500
Switzerland recorded the highest total salary cost among the countries shown, while Kuwait recorded the lowest.
Business Insight: Country-level salary costs help management understand how payroll expenditure is distributed geographically. These totals should be considered alongside employee counts and average salaries when evaluating payroll differences.
4.10 Workforce Gap Analysis
A RIGHT JOIN was used to identify job records without a matching employee record.
The result grid returned no records.
Business Insight: No unmatched job records were identified by this query in the result shown. This provides a useful database-checking step for reviewing the relationship between job records and employee records.
5. Recommendations
Based on the analysis, the following recommendations are proposed:
1.	Review workforce concentration: Examine staffing levels in Departments 50 and 80 to ensure that employee distribution supports operational requirements.
2.	Review salary distribution: Investigate the large number of employees within the low salary band and assess compensation in relation to job responsibilities and experience.
3.	Evaluate departmental compensation: Review departments with lower average salaries to understand differences in job composition and salary structure.
4.	Support salary benchmarking: Use job-role salary results to compare compensation across leadership and managerial positions.
5.	Strengthen workforce planning: Use departmental employee counts and country-level workforce information to support staffing and resource allocation.
6.	Monitor payroll expenditure: Compare country-level salary costs with employee counts to understand geographical differences in payroll spending.
7.	Maintain accurate workforce records: Continue checking employee and job records to identify unmatched or incomplete information.
6. Conclusion
The Orion Data Systems Workforce Analytics project demonstrated how SQL can be used to analyse employee data and generate meaningful workforce insights.
Using aggregation, filtering, subqueries, joins, CASE statements, and window functions, the analysis examined workforce distribution, salary bands, departmental leadership, job-role compensation, employee salary ranking, and country-level salary costs.
The findings highlighted employee concentration in key departments, differences in salary distribution, and variations in payroll costs across countries.
Overall, this project strengthened my practical SQL skills and demonstrated how database analysis can support human resource management, compensation review, and workforce planning.
7. Tools and SQL Skills
Tool: MySQL Workbench
SQL techniques used:
•	SELECT and WHERE
•	GROUP BY and ORDER BY
•	Aggregate functions: COUNT(), SUM(), AVG()
•	CASE statements
•	Subqueries
•	INNER JOIN, LEFT JOIN, and RIGHT JOIN
•	HAVING clause
•	Common Table Expressions (CTEs)
•	Window functions: ROW_NUMBER()




## Tools Used

**MySQL:** Used for querying, analysing, and extracting insights from the workforce database.
**MySQL Workbench:** Used as the database management and SQL development environment.
**SQL Techniques:** Used for data retrieval, aggregation, joins, subqueries, CTEs, CASE statements, and window functions.

## Conclusion

- The Orion Data Systems Workforce Analytics project demonstrated how SQL can be used to transform employee data into meaningful workforce insights.
- Through aggregation, filtering, subqueries, joins, CASE statements, and window functions, the analysis examined employee distribution, salary bands, departmental leadership, job-role compensation, employee rankings, and country-level salary costs.
- The findings highlighted workforce concentration in key departments, a larger population of employees within the low and medium salary bands, and differences in salary expenditure across countries.
- Overall, this project strengthened my practical SQL skills and demonstrated how database analysis can support human resource management, compensation review, and workforce planning.

