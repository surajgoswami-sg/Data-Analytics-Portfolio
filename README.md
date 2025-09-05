# Data Analytics Portfolio

A collection of my data analysis projects demonstrating foundational skills in data cleaning, exploratory analysis, and SQL.

---

## 1. E-commerce Sales Data Cleaning

* **Tools Used:** Google Sheets, `TRIM()`, `PROPER()`
* **Objective:** To clean and prepare a raw dataset of 1000 supermarket sales transactions for analysis.
* **Process:**
    * Loaded the raw `.csv` data into Google Sheets.
    * Created new columns to clean and standardize text fields, correcting inconsistencies in capitalization and removing hidden whitespace.
    * Used the "Copy -> Paste Special -> Values only" method to create a final, clean dataset with reliable data integrity.
* **Outcome:** Successfully transformed a raw, messy dataset into a structured and clean format, making it ready for reliable analysis.

---
## 2. Customer Behavior Analysis & Visualization

* **Tools Used:** Google Sheets, Pivot Tables, Charts
* **Objective:** To analyze the clean sales data to identify purchasing patterns across different customer segments.
* **Process:**
    * Created a Pivot Table to summarize 1000 sales transactions, counting payment method usage for both 'Member' and 'Normal' customer types.
    * Analyzed the aggregated data to extract a key business insight: Member customers prefer 'Cash', while Normal customers prefer 'Ewallet'.
    * Designed a stacked column chart to visually communicate this finding in a clear and professional format.
* **Outcome:** Translated raw data into an actionable business insight, providing a clear view of customer preferences.
* ### Final Visualization:
<img width="800" height="456" alt="image" src="https://github.com/user-attachments/assets/f8f2fc86-24c1-4c92-8953-b330311461e8" />



---
## 3. Business Database Querying with SQL

* **Tools Used:** SQL (`SELECT`, `TOP`, `COUNT`, `FROM`, `GROUP BY`, `ORDER BY`)
* **Objective:** To write foundational SQL queries to retrieve specific information and answer business questions from a sample database.
* **Process:**
    * Wrote a `SELECT...FROM...WHERE` query to retrieve a filtered list of customers from a specific country.
    * Wrote a more advanced query using `COUNT`, `GROUP BY`, and `ORDER BY` to calculate, aggregate, and rank customers by order volume.
    * Successfully debugged and adapted a query to use the `TOP` clause, which is specific to the SQL Server dialect.
* **Outcome:** Successfully queried a database to extract key business information, demonstrating an understanding of core SQL commands and syntax. The final query to find the top customers was:
    ```sql
    SELECT TOP 5
        CustomerID,
        COUNT(OrderID)
    FROM
        Orders
    GROUP BY
        CustomerID
    ORDER BY
        COUNT(OrderID) DESC;
    ```
