# 📊 Sales Analysis Project (Python + SQLite)

This project demonstrates how to analyze basic sales data using **Python**, **SQLite**, **Pandas**, and **Matplotlib**. It also includes essential SQL queries to perform key summaries and generate visual insights.

---

## ✅ Objective

- Connect to a local SQLite database
- Query total sales quantity and revenue by product
- Visualize sales revenue using a bar chart
- Practice basic SQL for data exploration

---

## 🛠️ Tools Used

- Python (with `sqlite3`, `pandas`, `matplotlib`)
- SQLite (local database)
- Jupyter Notebook or .py script

---

## 🗂️ Database Setup

### Table Structure: `sales`

```sql
CREATE TABLE sales (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    product TEXT NOT NULL,
    quantity INTEGER NOT NULL,
    price REAL NOT NULL
);
