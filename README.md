🗄️ SQL Retail & Sales Data Analysis Project | Data Technician Bootcamp
🚀 Project Overview
This project was completed as part of a Data Technician Bootcamp and focused on using SQL (Structured Query Language) to extract, manipulate, and analyse retail and sales data stored in relational databases.

The project involved writing SQL queries to explore customer, product, order, and sales datasets, enabling the identification of trends, performance metrics, and actionable business insights. By working with multiple related tables, I developed practical experience in querying databases and transforming raw data into meaningful information for reporting and decision-making.

🛠️ Skills Demonstrated
🔍 Data Retrieval with SELECT
Used SELECT statements to retrieve and analyze specific datasets, including:

📋 Extracting customer, product, and sales records
🎯 Selecting relevant columns for reporting
🔎 Querying business-critical information
📊 Exploring large retail and sales datasets
Example Skills:

SELECT ProductName, SalesAmount
FROM Sales;
🎛️ Data Filtering with WHERE
Applied WHERE clauses to focus on specific business requirements and data subsets.

✅ Filtered products by category
💰 Identified high-value sales transactions
📅 Retrieved records within specific date ranges
👥 Examined customer segments
Example Skills:

SELECT *
FROM Sales
WHERE SalesAmount > 1000;
🔽 Data Sorting with ORDER BY
Organized data to highlight trends and top-performing areas.

📈 Ranked products by sales performance
💰 Sorted revenue from highest to lowest
📊 Ordered customer activity levels
🛍️ Identified best-selling products
Example Skills:

SELECT ProductName, SalesAmount
FROM Sales
ORDER BY SalesAmount DESC;
📊 Data Aggregation with GROUP BY
Used aggregation functions to summarize and analyze business performance.

💰 Total sales by product category
📦 Product performance analysis
🌍 Regional sales comparisons
👥 Customer purchasing patterns
📈 Sales trend reporting
Common Functions Used:

SUM()
AVG()
COUNT()
MIN()
MAX()
GROUP BY
Example Skills:

SELECT Category, SUM(SalesAmount)
FROM Sales
GROUP BY Category;
🔗 Table Relationships & JOINs
Combined data from multiple tables to gain deeper business insights.

INNER JOIN
Matched related records across tables.

SELECT Customers.CustomerName,
       Orders.OrderID
FROM Customers
INNER JOIN Orders
ON Customers.CustomerID = Orders.CustomerID;
LEFT JOIN
Retrieved all records from one table while matching available records from another.

RIGHT JOIN
Returned all records from the secondary table with matching primary table data.

FULL OUTER JOIN
Combined all available records from multiple datasets.

Business Applications:

👥 Customer and order analysis
📦 Product and category reporting
🚚 Supplier and inventory tracking
💰 Sales and revenue analysis
📊 Comprehensive business reporting
🛍️ Retail & Sales Data Analysis
💰 Sales Performance Analysis
Identified top-performing products
Calculated total revenue by category
Analyzed sales trends over time
Compared product performance
👥 Customer Analysis
Examined purchasing behavior
Identified valuable customer segments
Analyzed order frequency
Explored customer spending patterns
📦 Product Analysis
Measured product popularity
Compared category performance
Investigated inventory trends
Tracked product sales growth
🌍 Regional Analysis
Compared sales across locations
Identified high-performing regions
Analyzed geographic sales distribution
Supported location-based business decisions
📈 Reporting & Business Intelligence
Generated SQL queries to support:

📊 Performance Dashboards
📈 Sales Trend Reporting
💰 Revenue Analysis
🎯 KPI Monitoring
📋 Business Intelligence Reporting
🔍 Data-Driven Decision Making
🛠️ Tools & Technologies
🗄️ SQL
🐘 PostgreSQL / SQL Databases
💻 SQL Query Editors
📊 Relational Databases
📋 Database Management Systems (DBMS)
📈 Data Analytics & Reporting
🎯 Learning Outcomes
Through this project, I gained practical experience in:

✅ Writing SQL Queries
✅ Data Extraction & Retrieval
✅ Data Filtering & Sorting
✅ Aggregating Data with GROUP BY
✅ Using SQL Functions (SUM, AVG, COUNT)
✅ Performing Table JOINs
✅ Database Relationships
✅ Retail & Sales Analytics
✅ Business Reporting
✅ Data Analysis & Problem Solving
✅ Data-Driven Decision Making

#WORLD Database
Cities with Population Larger than 2,000,000: Scenario: A real estate developer is interested in cities with substantial population sizes for potential investment opportunities. You're tasked with identifying cities from the database with populations exceeding 2 million to focus their research efforts.
SELECT name, countrycode, population
FROM city
where population > '2000000'
ORDER by population desc

Cities in Europe: Scenario: A European cultural exchange program is seeking to connect students with cities across the continent. You're tasked with compiling a list of cities located in Europe from the database to facilitate program planning and student engagement.
SELECT City.Name, Country.Name
FROM City
JOIN Country
ON City.CountryCode = Country.Code
WHERE Country.Contitent = 'Europe';

Display Columns with Limit (Rows 31-40): Scenario: A market research firm requires detailed information on cities beyond the top rankings for a comprehensive analysis. You're tasked with providing data on cities ranked between 31st and 40th by population to ensure a thorough understanding of urban demographics.
SELECT Name, Population
FROM City
ORDER BY Population DESC
LIMIT 30,10;

#Northwind Database
Retrieve Full Customer Data Your manager has asked you to export the full list of all customer details into a report. ➡️ Write a SQL query to retrieve all columns from the Customers table.
SELECT * 
FROM Customers; 

International Customers Targeting (USA & UK) The marketing team is preparing campaigns for customers in the USA and UK. ➡️ Write a SQL query to retrieve all columns from the Customers table where the Country is either 'USA' or 'UK'.
SELECT * 
FROM Customers 
WHERE Country = ‘USA’ OR Country = 'UK';

📘 Complete Order Overview The business team wants to see a detailed order list with customer and employee information. ➡️ Write a SQL query to retrieve the Order ID, Order Date, Customer Name, and Employee Name for all orders.
SELECT o.orderID, o.orderDate, c.CompanyName AS CustomerName, 
FROM orders o  
INNER JOIN Customers c 
ON o.customerID = c.CustomerID 
INNER JOIN Employees e 
ON o.EmployeeID = e.EmployeeID; 


🌟 Project Outcome
This project strengthened my ability to use SQL to transform raw retail and sales data into meaningful business insights. By applying SELECT, WHERE, ORDER BY, GROUP BY, and JOIN operations, I developed the skills needed to efficiently query databases, analyze performance metrics, and support business intelligence reporting.

The project demonstrates my ability to work with relational databases and leverage SQL to uncover trends, answer business questions, and drive informed decision-making through data. 🚀📊🗄️
