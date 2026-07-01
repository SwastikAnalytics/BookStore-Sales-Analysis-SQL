# 📚 Book Store Sales Analysis using SQL (PostgreSQL)

A SQL-based data analysis project that explores bookstore sales, customer purchasing behavior, inventory management, and revenue insights using PostgreSQL.

The project demonstrates how SQL can be used to solve real-world business problems by analyzing transactional data and generating meaningful business insights.

---

## 📑 Table of Contents

- [Project Overview](#-project-overview)
- [Business Problem](#-business-problem)
- [Project Objectives](#-project-objectives)
- [Database Schema](#-database-schema)
- [Entity Relationship Diagram](#-entity-relationship-diagram)
- [Dataset](#-dataset)
- [Tools & Technologies](#-tools--technologies)
- [Project Structure](#-project-structure)
- [SQL Concepts Used](#-sql-concepts-used)
- [Business Questions Solved](#-business-questions-solved)
- [Key Business Insights](#-key-business-insights)
- [How to Run the Project](#-how-to-run-the-project)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

# 📖 Project Overview

This project simulates the operations of a bookstore by managing books, customers, and sales transactions in a relational database.

Using PostgreSQL, various SQL queries are written to analyze:

- Customer purchasing behavior
- Book sales performance
- Inventory status
- Revenue generation
- Genre popularity
- Top customers
- Business KPIs

---

# 🎯 Business Problem

Bookstores generate thousands of sales transactions that contain valuable information about customers, books, and purchasing behavior.

Without proper analysis, businesses cannot easily identify:

- Best-selling books
- Low-performing books
- Customer spending patterns
- Inventory shortages
- Revenue trends
- Genre performance

This project uses SQL to transform raw transactional data into meaningful business insights for better decision-making.

---

# 🚀 Project Objectives

- Design a relational bookstore database
- Perform data analysis using SQL
- Analyze customer purchasing behavior
- Monitor inventory levels
- Calculate revenue
- Identify top-selling books
- Find loyal customers
- Generate business reports

---

# 🗄 Database Schema

The database contains three tables.

## Books

| Column | Data Type |
|----------|------------|
| Book_ID | SERIAL (PK) |
| Title | VARCHAR(100) |
| Author | VARCHAR(100) |
| Genre | VARCHAR(50) |
| Published_Year | INT |
| Price | NUMERIC(10,2) |
| Stock | INT |

---

## Customers

| Column | Data Type |
|----------|------------|
| Customer_ID | SERIAL (PK) |
| Name | VARCHAR(100) |
| Email | VARCHAR(100) |
| Phone | VARCHAR(15) |
| City | VARCHAR(50) |
| Country | VARCHAR(150) |

---

## Orders

| Column | Data Type |
|----------|------------|
| Order_ID | SERIAL (PK) |
| Customer_ID | INT (FK) |
| Book_ID | INT (FK) |
| Order_Date | DATE |
| Quantity | INT |
| Total_Amount | NUMERIC(10,2) |

---

# 📊 Entity Relationship Diagram


```

---

# 📂 Dataset

The project contains three datasets.

| File |
|------|
| Books |
| Customers |
| Orders |

---

# 🛠 Tools & Technologies

| Tool | Purpose |
|-------|----------|
| PostgreSQL | Database |
| SQL | Data Analysis |
| pgAdmin | Query Execution |
| Git | Version Control |
| GitHub | Project Hosting |

---

# 📁 Project Structure

```
BookStore-Sales-Analysis-SQL
│
├── README.md
├── BookStore_SQL_Project_PPT
├── BookStore_SQL_Project_Report
|
|
├── Database
│   ├── create database.txt
│
├── Queries
│   ├── 01_Basic_Queries.txt
│   ├── 02_Aggregate_Functions.txt
│   ├── 03_Joins.txt
│   ├── 04_Business_Insights.txt
│   └── 05_Advanced_Queries.txt
│
├── Dataset
│   ├── Books.csv
│   ├── Customers.csv
│   └── Orders.csv
│
├── Diagram
│   └── E-R Diagram
│ 
    
```

---

# 💡 SQL Concepts Used

- SELECT
- WHERE
- ORDER BY
- GROUP BY
- HAVING
- LIMIT
- DISTINCT
- Aggregate Functions
- INNER JOIN
- LEFT JOIN
- Foreign Keys
- Primary Keys
- COALESCE
- SUM()
- AVG()
- COUNT()

---

# 📈 Business Questions Solved

✔ Retrieve all Fiction books

✔ Find books published after 1950

✔ Calculate total revenue

✔ Find the most expensive book

✔ Find the lowest stock book

✔ Identify top spending customers

✔ Find repeat customers

✔ Calculate remaining inventory

✔ Analyze genre-wise sales

✔ Find the most frequently ordered book

✔ Analyze author-wise sales

✔ Find customers with multiple orders

✔ Calculate average book prices

✔ Track inventory after sales

---

# 📊 Key Business Insights

- Total revenue generated from bookstore sales
- Most popular book genres
- Best-selling books
- Top spending customers
- Inventory remaining after orders
- Customer purchasing frequency
- Author-wise sales performance
- Genre-wise sales analysis
- Books requiring stock replenishment

---

# ▶ How to Run the Project

### Clone Repository

```bash
git clone https://github.com/yourusername/BookStore-Sales-Analysis-SQL.git
```

### Open PostgreSQL

Open pgAdmin 

### Execute SQL Files

Run in the following order:

```
01_Create_Tables.sql

↓

02_Import_Data.sql

↓

03_View_Data.sql

↓

Queries/
```

---

# 🚀 Future Improvements

- Create SQL Views
- Add Stored Procedures
- Implement Triggers
- Build Power BI Dashboard
- Add Monthly Sales Reports
- Develop Interactive Business Reports

---

# 👨‍💻 Author

**Swastik Kumar**

Computer Engineering Student

SQL | PostgreSQL | Power BI | Excel | Python

GitHub: https://github.com/yourusername

LinkedIn: https://linkedin.com/in/yourprofile

