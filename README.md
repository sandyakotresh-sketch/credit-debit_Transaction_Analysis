💳 Card Transactions Analysis Dashboard
🧩 Overview

This project presents a comprehensive Card Transactions Analysis Dashboard built using Power BI.
The data was generated and cleaned using SQL, simulating real-world transaction records.
The dashboard provides key insights into customer spending behavior, transaction patterns, and performance metrics using DAX formulas and interactive visualizations.

🖼️ Dashboard Preview

(Replace with your actual screenshot images)

Overview Page	Customer Insights	Transaction Analysis

	
	
📊 Dataset

Dataset was created in SQL using AI prompts from Perplexity to simulate realistic card transaction data.

Data cleaning, transformation, and validation were performed in SQL before loading into Power BI.

Tables Used:

Customers – Customer demographics and personal details

Accounts – Account type, balance, and customer linkage

Transactions – Transaction ID, date, amount, and type

⚙️ Tools & Technologies
Tool / Technology	Purpose
SQL Server	Data generation, cleaning, and transformation
Power BI	Data visualization and dashboard creation
DAX (Data Analysis Expressions)	For calculations, KPIs, and measures
Perplexity AI	Used for AI-driven random data generation

📐 DAX Formulas Used
Total Transaction Amount
Total Transaction Amount = SUM(Transactions[Amount])

Average Transaction Value
Average Transaction = AVERAGE(Transactions[Amount])

Total Customers
Total Customers = DISTINCTCOUNT(Customers[CustomerID])

Customer Age Group
Customer Age Group = SWITCH(
    TRUE(),
    [Customer Age] <= 25, "≤25",
    [Customer Age] <= 35, "26-35",
    [Customer Age] <= 50, "36-50",
    "51+"
)

Transaction Count
Transaction Count = COUNT(Transactions[TransactionID])

🧠 Prerequisites

Before opening or using this project:

Install Power BI Desktop (latest version).

Have SQL Server Management Studio (SSMS) if you wish to recreate or inspect the data.

Clone or download this repository.

Open Card_Transactions.pbix in Power BI Desktop.

🔍 Key Insights

Found top-performing transaction categories and peak spending periods.

Identified high-value customers and frequent spenders.

Analyzed customer age group vs. spending patterns.

Detected monthly and yearly transaction trends.

Provided a clear overview of total revenue, average transaction value, and customer distribution.

❓ Analytical Questions Addressed

What is the total transaction amount and average transaction per customer?

Which age group contributes the most to revenue?

What are the top transaction categories?

Which customers or accounts have the highest transaction frequency?

What are the month-on-month spending trends?

🏁 Conclusion

This Power BI project demonstrates how to:

Generate, clean, and prepare data using SQL.

Apply DAX formulas for in-depth analysis.

Create a dynamic, interactive Power BI dashboard for financial insights.

It reflects an end-to-end data analytics workflow — from data creation → cleaning → analysis → visualization.

