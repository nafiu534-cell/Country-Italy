# Country-Italy
This project presents an exploratory data analysis (EDA) on a real-world retail dataset using Python. The analysis focuses on uncovering patterns in customer transactions, identifying anomalies and trends, and understanding the relationships between various features in the dataset. Visualizations are used extensively to reveal distribution, skewness, and time-based patterns in the data.

**Dataset Description**

The dataset consists of transaction records from a UK-based online retail store over the course of one year (December 2010 – December 2011). Key features include:

InvoiceNo – Unique identifier for each transaction

StockCode – Unique product code

Description – Product name

Quantity – Number of items purchased

InvoiceDate – Date and time of the transaction

UnitPrice – Price per unit

CustomerID – Unique ID assigned to each customer

Country – Customer’s country

**Tools and Libraries**


pandas for data manipulation

numpy for numerical operations

matplotlib & seaborn for data visualization

 **Analysis Workflow**

 1. Data Cleaning & Preprocessing
Removed duplicated entries (5,268 rows)

Handled missing values in CustomerID and Description

Removed transactions with unspecified countries

Filtered out anomalies in StockCode (e.g., ‘POST’, ‘BANK CHARGES’)

Created additional columns for analysis (e.g., InvoiceMonth, Transaction Status)

Labeled transactions as canceled or completed based on Quantity values

**2. Feature Exploration & Visualization**
Examined the distribution of key numerical columns using histograms and boxplots

Identified outliers using IQR (Interquartile Range) method

Investigated skewness and spread in Quantity and UnitPrice

Analyzed product performance by:

Top 10 most purchased items

Top 10 most frequently occurring products

**3. Country-Based Insights**

Counted the number of transactions by country

Filtered and analyzed all retail activity in Italy, with specific attention to:

Top products sold

Most expensive items

Product trends and purchasing patterns

**4. Time Series Analysis**
Extracted temporal features from InvoiceDate: InvoiceDay, InvoiceHour, InvoiceMonth, etc.

**Visualized:**

Total sales by month

Sales patterns by day of the week and hour of the day

Monthly sales trends for the top 5 products in Italy

**Key Insights**
The United Kingdom had the highest transaction volume, followed by Germany and France.

Negative quantities indicated returns or canceled orders, allowing for the classification of transaction statuses.

High standard deviations and outliers in Quantity and UnitPrice signaled unusual purchases or potential errors.

Italy's consumer behavior exhibited peak sales in November and high activity during weekday afternoons.

Several products consistently dominated sales across months, hinting at top-performing stock.
