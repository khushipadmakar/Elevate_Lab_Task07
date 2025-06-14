# Elevate_Lab_Task07
📊 Sales Analysis with SQLite and Python
This mini-project demonstrates how to use SQLite, Pandas, and Matplotlib in Python to perform simple sales data analysis.

✅ Objectives
Connect to an SQLite database (sales_data.db)

Query the database to calculate:

Total quantity sold per product

Total revenue per product

Display results using pandas

Visualize revenue by product using a bar chart

🧰 Tools & Technologies
Python

SQLite (via sqlite3)

pandas

matplotlib

📁 Dataset
The database contains a single table called sales with the following structure:

Column	Type	Description
id	INTEGER	Primary Key
product	TEXT	Name of the product
quantity	INTEGER	Quantity sold
price	REAL	Price per unit

📜 SQL Query Used
sql
Copy
Edit
SELECT product, 
       SUM(quantity) AS total_qty, 
       SUM(quantity * price) AS total_revenue 
FROM sales 
GROUP BY product;
📈 Output
The script prints a summary DataFrame in the terminal

A bar chart (sales_chart.png) is generated showing revenue by product

🚀 How to Run
Ensure you have Python and the required libraries installed:

bash
Copy
Edit
pip install pandas matplotlib
Run the script:

bash
Copy
Edit
python sales_analysis.py
Output will include:

Printed DataFrame

Saved chart image: sales_chart.png

📌 Example Output
mathematica
Copy
Edit
  product  total_qty  total_revenue
0   Apple         15           37.5
1  Banana         30           30.0
2  Orange         20           30.0
Bar chart visualizes this data.
