FNP Sales Analysis – Excel Dashboard Project
📊 End-to-End Data Analytics Project (Excel • Power Query • Power Pivot • DAX)

This project analyzes sales data from FNP (Ferns & Petals) to uncover insights related to revenue patterns, customer behavior, product performance, monthly sales trends, and operational efficiency.

📁 Project Overview

FNP is a gifting platform specializing in occasions such as Diwali, Birthdays, Holi, Raksha Bandhan, Valentine’s Day, and Anniversaries.
The goal of this project was to analyze their 2023 order data, build a clean data model, generate KPIs, and design an interactive Excel dashboard answering major business questions.

✔️ Business Questions Solved

Total Revenue

Average Order-to-Delivery Time

Monthly Sales Performance (2023)

Top Products by Revenue

Average Customer Spending

Top 5 Product Sales Performance

Top 10 Cities by Order Volume

Impact of Order Quantity on Delivery Time

Revenue by Occasion

Product Popularity by Occasion

🛠 Tools & Techniques Used

Excel

Power Query (Data Transformation)

Power Pivot (Data Modeling)

DAX for calculated columns

Data Visualization (Excel Dashboard)

🔄 Project Workflow
1. Data Extraction

Imported four datasets into Excel:

Customers

Orders

Products

Dates

2. Data Cleaning

Very minimal cleaning was required.
✔ Changed contactnumber datatype from Whole Number → Text.

3. Data Transformation (Power Query)

Performed the following transformations in the Orders table:

Created Month Name from order_date

Created Hour (Order Time) from order_time

Created Hour (Delivery Time) from delivery_time

Created diff_order_delivery = Delivery Date – Order Date

Converted result to Whole Number

Merged Price column from Products table using
Left Join → product_id key

4. Data Modeling (Power Pivot)

A Star Schema was built:

Customers → Orders

Products → Orders

No existing relationships were present; all were manually created.

5. DAX Calculations

Created additional columns in Power Pivot:

✔ Revenue
Revenue = Price * Quantity

✔ Day Name
Day Name (Order_Date) = FORMAT(order_date, "DDDD")


These enabled advanced time-based and revenue-based analytics.

6. Data Analysis

Key findings:

Total Revenue: ₹35,20,984

Total Orders: 1000

Avg. Order-to-Delivery Time: 5.53 days

Avg. Customer Spend: ₹3,520.98

Top Revenue Months: March & August

Top Categories: Cake, Soft Toys

Top Cities: Dibrugarh, Imphal, Gunakal

Correlation (Order Quantity vs Delivery Time):
0.003478174 → No relationship
(Higher order quantity does not impact delivery time)

7. Dashboard

An interactive Excel dashboard was created showing:

KPIs

Revenue by Occasion

Revenue by Category

Top 10 Cities

Revenue by Month

Top 5 Products

Revenue by Hour

Slicers for filtering by date & occasion

Screenshot of dashboard is included in the repository.

📌 Final Insights

FNP’s sales peak around festive seasons and special occasions, especially Anniversary and Raksha Bandhan.

No operational delay caused by larger orders.

Strong product categories like Cakes and Soft Toys are major revenue drivers.

City-level ordering patterns show clear hotspots, helping in targeted marketing.
