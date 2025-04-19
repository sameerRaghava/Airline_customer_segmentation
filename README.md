# Airline Customer Segmentation using SQL
This project showcases how SQL can be used to extract meaningful insights from a structured relational database. By writing optimized queries, I analyzed customer purchasing behavior, revenue trends, and product popularity. Key operations involved data filtering, joining multiple tables, aggregation, and using window functions. The project highlights strong foundational skills in SQL for data analysis and reporting.

  # 🗃️ Sales and Customer Analytics using SQL

## 🔍 Project Overview
This project focuses on exploring a sales database using SQL. It includes writing queries to analyze product performance, customer demographics, and revenue generation. The results help in understanding sales drivers and optimizing marketing strategies.

## 🛠 Tools & Environment
- MySQL / PostgreSQL / SQL Server (adjust based on what you used)
- SQL Workbench / pgAdmin / Azure Data Studio
- Sample Database (e.g., AdventureWorks, or a custom dataset)

## 💡 Key Queries & Use Cases
- Top 10 best-selling products by revenue
- Monthly sales trends
- Customer segmentation based on purchase frequency
- Join operations to combine product, order, and customer info
- Window functions to rank customer spending behavior

## 📁 Project Files
- `queries/`: SQL query scripts (.sql or .txt)
- `results/`: Screenshots or CSVs of query outputs (optional)
- `README.md`: This documentation

## ✅ Skills Demonstrated
- Data extraction using SELECT, JOIN, GROUP BY, ORDER BY
- Aggregate functions (SUM, COUNT, AVG)
- Subqueries and nested filters
- Window functions (ROW_NUMBER, RANK, etc.)
- Translating business questions into SQL queries

## 📌 Sample Query

```sql
-- Top 5 revenue-generating products
SELECT product_name, SUM(total_amount) AS revenue
FROM sales
GROUP BY product_name
ORDER BY revenue DESC
LIMIT 5;
