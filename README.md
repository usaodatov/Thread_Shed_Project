 Thread Shed Sales Analysis

This project processes and analyzes a daily sales report for a fictional shop called Thread Shed. The goal is to clean and organize the sales data, compute total sales, and provide insights into the types and quantities of threads sold.

---

 Project Overview

The `daily_sales` string contains raw, unstructured data about:
- Customers: Names of the customers.
- Sales: Total amount of money spent by each customer.
- Thread Sold: Thread colors purchased by customers.

The project involves:
1. Cleaning and formatting the raw data.
2. Extracting and organizing specific details like customer names, sales amounts, and thread colors sold.
3. Calculating total sales for the day.
4. Analyzing thread sales by color.

---

 Technologies Used

- Python: Core language for data processing and analysis.
- String Manipulation: Methods like `.replace()`, `.split()`, and `.strip()` were used to clean and parse the data.
- Data Structures: Lists and nested lists to organize and process the cleaned data.

---

 Project Workflow

 1. Cleaning the Raw Data
- Replaced inconsistent delimiters (`;,;`) with a cleaner separator (`-`).
- Split the cleaned data into individual transactions using `.split()`.

 2. Parsing Transactions
- Further split each transaction into:
  - Customer Name
  - Sale Amount
  - Thread Colors Sold
- Cleaned unnecessary whitespace and newline characters from all entries.

 3. Extracting Key Insights
- Customers: A list of all customers who made purchases.
- Sales: A list of all sales amounts in dollar values.
- Thread Sold: A breakdown of all thread colors purchased, including multi-colored items (split into individual colors).

 4. Computing Total Sales
- Calculated the total revenue for the day by summing up the cleaned sales amounts.

 5. Analyzing Thread Sales by Color
- Provided a function, `color_count(color)`, to count the number of items sold for any specific thread color.

---

 Key Functions

 `color_count(color)`
- Description: Takes a color as input and returns the total number of threads sold in that color.
- Example Usage:
  ```python
  color_count('white') 
   Output: Total of X white items sold.
