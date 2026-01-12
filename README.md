# 🛒 Sales Data Warehouse Project

![Status](https://img.shields.io/badge/Status-Completed-success)
![SQL](https://img.shields.io/badge/Language-T--SQL-blue)
![Architecture](https://img.shields.io/badge/Architecture-Medallion-purple)

## 👋 Introduction
Welcome to my SQL Data Warehouse project! I built this project to practice **Data Engineering** skills and understand how to transform raw business data into meaningful insights.

The goal was to take messy CSV files from two different systems (ERP and CRM), clean them up, and build a structured Data Warehouse capable of answering business questions.

## 🎯 What I Built
I simulated a real-world scenario where a company needs to analyze their sales performance.
* **ETL Pipeline:** I built a process to extract data, clean it, and load it into a Data Warehouse.
* **Data Modeling:** I designed a Star Schema (Fact and Dimensions) to make reporting easy and fast.
* **Data Quality:** I focused on fixing issues like null values, duplicates, and inconsistent formatting.

## 🛠️ Architecture (Medallion)
I followed the **Medallion Architecture** (Bronze, Silver, Gold) because it keeps the data organized:

* **🥉 Bronze Layer:** Holds the raw data exactly as it came from the source (CSV files).
* **🥈 Silver Layer:** This is where the cleanup happens. I standardized date formats and merged data from ERP and CRM.
* **🥇 Gold Layer:** The final data model ready for analysis. I created a Fact table for sales and Dimension tables for Products and Customers.

## 🔎 Key Insights
After building the warehouse, I wrote SQL queries to find answers to:
* Who are our best customers? (RFM Analysis)
* Which product categories are selling the best?
* How are sales growing year over year?

## 💻 Tech Stack
* **Database:** Microsoft SQL Server
* **Language:** T-SQL
* **Concepts Used:** ETL, Data Cleaning, Star Schema, Primary/Foreign Keys, Window Functions.

## 🚀 How to Run
1.  Clone this repo.
2.  Run `scripts/init_database.sql` to create the database.
3.  Execute the scripts in the `scripts/` folder in order (Bronze -> Silver -> Gold).
4.  Check out the queries in `analytics/` to see the results!
