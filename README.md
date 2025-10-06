# AirlineDB SQL Project (PostgreSQL)

📘 Overview

The AirlineDB SQL Project demonstrates how to use SQL for real-world data analysis using an airline database. The dataset simulates booking transactions, flight schedules, airports, and store sales. This notebook is structured to guide users through a set of practical SQL problems, focusing on aggregation, ranking, date formatting, and joins.

🧩 Database Description

The AirlineDB schema typically includes the following tables:

bookings: Contains booking reference, booking date, and total amount.

tickets: Stores individual ticket information linked to bookings.

boarding_passes: Contains information about passengers who checked in.

flights: Stores flight schedules, departure, and arrival airports.

stores, products, sales: Represent a commercial component used for sales analysis.

🎯 Problem Statements & Objectives
1️⃣ Tickets Without Boarding Passes

Goal: Count how many tickets do not have a corresponding boarding pass.
Key SQL Concepts: LEFT JOIN, IS NULL.

2️⃣ Format Booking Date

Goal: Display the book_date column in the format yyyy-mm-dd along with book_ref and total_amount.
Key SQL Concepts: TO_CHAR(), column aliasing.

3️⃣ Most Popular Product in Each Store

Goal: Identify the most sold product (by quantity) per store.
Key SQL Concepts: GROUP BY, SUM(), RANK() OVER().

4️⃣ Quarterly Store Performance Ranking

Goal: Calculate total sales per store for each quarter and rank stores based on performance.
Key SQL Concepts: Window functions, TO_CHAR() date formatting, CTEs.

5️⃣ Airport Ranking by Departures

Goal: Rank airports based on the number of departing flights.
Key SQL Concepts: COUNT(), RANK(), GROUP BY.

🧠 Skills Demonstrated

SQL joins and aggregations

Window functions (RANK, PARTITION BY)

Date formatting and manipulation

Data summarization for business insights

🛠️ Environment

Database: PostgreSQL

Notebook Tool: Jupyter Notebook (%sql magic or PostgreSQL kernel)

🚀 How to Run

Install PostgreSQL and Jupyter.

Load the AirlineDB schema and data.

Open AirlineDB_SQL_Project.ipynb in Jupyter.

Run each SQL cell to view the query results.

📈 Expected Output

Each query returns either:

A single aggregated number, or

A ranked table with columns exactly as specified in each problem.

👨‍💻 Author

Created by Vicky as part of an SQL learning and data analysis showcase using PostgreSQL.
