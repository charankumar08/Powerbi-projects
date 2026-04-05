# 📊 Insurance Analytics Dashboard (End-to-End)

## 📝 Project Overview
This project provides a comprehensive business intelligence solution for **Prism Insurance Pvt. Ltd.** to monitor policy performance, claims distribution, and customer demographics. It demonstrates a full data lifecycle: from hosting a relational database in **SQL Server** to deploying an automated, secure dashboard in the **Power BI Service**.

## 🛠️ Technical Workflow
* **Data Sourcing:** Integrated a hybrid data environment using **SQL Server** (Relational Database), local **CSV** files (Insurance Records), and **Excel** (Customer Feedback).
* **Data Modeling & ETL:** Conducted data cleaning and schema modeling in **Power Query** to ensure data integrity across multiple sources without relying on complex DAX for visuals.
* **Interactive Features:** * Implemented global **Slicers** for Policy, Claim, and Customer IDs.
    * Configured **Drill-through Filters** for "Premium Policy Type" to allow users to dive from high-level trends into specific policy details.
* **Advanced Analytics:** Implemented **Sentiment Analysis (Text Analytics)** on customer feedback data to evaluate service satisfaction and correlate it with claim statuses.
* **Security (RLS):** Built and validated a **Row-Level Security** framework to restrict data access by department.
* **Power BI Service:** Published to a personal workspace and configured **Scheduled Refresh** via an **On-premises Data Gateway (Personal Mode)**.

## 📈 Key Business Insights
* **Financial Summary:** Managed a portfolio with **$5.97M** in Total Premiums vs. **$16.90M** in Total Claims.
* **Top Performer:** **Travel Insurance** is the leading policy type, contributing **$2.5M** in revenue.
* **Claims Overview:** Analyzed 10,000 policies showing a distribution of **4.4K Rejected**, **3.4K Settled**, and **2.3K Pending** claims.
* **Demographics:** Identified that the **"Adult"** age group represents the highest financial risk, with **$8.8M** in total claim amounts.

## 🔐 Security Implementation (RLS)
To ensure data privacy between departments, I implemented DAX filters on the `PolicyType` table:
* **Travel Role:** `[PolicyType] = "Travel"`
* **Health Role:** `[PolicyType] = "Health"`
* *Validation:* Verified roles using the "View as" feature in Power BI Service to ensure users only see data relevant to their department.
* 
🚀 How to Run This Project
1. Database Setup (SQL Server)
Run the following script in SQL Server Management Studio (SSMS) to prepare your data source:

```text
CREATE DATABASE Insurancedb;
GO
USE Insurancedb;
GO
-- Import your CSV data into a table named 'InsuranceRecords'
SELECT TOP 10 * FROM InsuranceRecords;
```

### 2. Connect Power BI
1. Open `Prism_Insurance_Report.pbix` in **Power BI Desktop**.
2. Navigate to the **Home** tab, click **Transform Data** > **Data Source Settings**.
3. Select the SQL Server source and click **Change Source**.
4. Update the **Server** field to your local instance name:
   ```text
   Server: LAPTOP-6GDIGOSM\SQLEXPRESS
   Database: Insurancedb

## 📂 Repository Structure
```text
├── Data/
│   ├── insurance_data.csv          # Core insurance records (CSV)."
3.  Click **Commit changes**.
│   └── customer_feedback.xlsx     # Data for Sentiment Analysis (Excel)
├── SQL_Scripts/
│   └── database_setup.sql         # Script to recreate the SQL Server database
├── Prism_Insurance_Report.pbix     # Power BI Desktop File
├── Dashboard_Preview.pdf           # Static export of the final dashboard
└── README.md                       # Project documentation

