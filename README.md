# Data-Analyst-InternShip=Project7

# Task 7: Sales Summary with MySQL and Python

## Tools
- Python
- MySQL
- Pandas
- Matplotlib

## What I Did
- Created a MySQL database `sales_db` and a table `sales`
- Inserted sample data for products
- Wrote a SQL query to summarize total quantity and revenue
- Loaded the result into a Pandas DataFrame
- Visualized revenue per product using a bar chart

## SQL Query Used
```sql
SELECT product, 
       SUM(quantity) AS total_qty,
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product
