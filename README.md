Objectives:
TO Perform SQL queries on an E-commerce database to analyze customer orders, revenue, and sales trends.
Tools Used:
MySQL 
Dataset :
Database includes 3 main tables:
Customers → Customer details
Products → Product details with price
Orders → Order transactions
Tasks I performed:
Basic Queries – SELECT, WHERE, ORDER BY
Aggregations – SUM, AVG
GROUP BY – Analyze customer spending
JOINS – Combine Customers, Orders, Products
Subqueries – Find above-average spenders
Views – Monthly sales summary
One Sample Example Query:
-- Monthly sales totals (MySQL)
CREATE VIEW MonthlySales AS
SELECT DATE_FORMAT(OrderDate, '%Y-%m') AS Month, 
       SUM(o.Quantity * p.Price) AS TotalSales
FROM Orders o
JOIN Products p ON o.ProductID = p.ProductID
GROUP BY Month;
 Deliverables:
Screenshots of all query outputs.
 Outcome:
Learnt to manipulate and analyze structured data using SQL.
Performed  joins & aggregations.

Create views for reporting

Use indexes for performance
