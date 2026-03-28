
# 📊 Sales Performance & Promotion Analytics (End-to-End BI Project)

## 📖 Project Overview
This Power BI project provides a deep-dive analysis of a retail dataset containing over **3,510 orders**. The primary goal was to transform raw sales data into actionable business insights by tracking product performance, promotional effectiveness, and geographical sales distribution from **2020 to 2024**.

---

## 🎯 Business Requirements & Solutions
I designed this dashboard to solve **8 specific business problems** defined in the project brief:

1.  **Top/Bottom 5 Analysis:** 
    *   Identified **Apple iPhone 14** as the top revenue driver (**21.4M**) and **Colgate Toothpaste** as the lowest (**0.02M**).
2.  **Sales Trends Over Time:** 
    *   Visualized fluctuations across Daily, Monthly, and Annual periods. A notable peak occurred in 2023 (**32M**) followed by a sharp decline in early 2024.
3.  **Sales vs. Profit Relationship:** 
    *   Used a scatter plot to confirm a strong linear correlation between Net Sales and Profit, ensuring pricing strategies are consistent.
4.  **Period-over-Period (PoP) Comparison:** 
    *   Developed a custom **"Dual-Date Slicer"** system (Page 3 & 4) allowing stakeholders to compare Sales, Profit, and Quantity between any two custom time ranges side-by-side.
5.  **Average Discount Analysis:** 
    *   Analyzed 5 promotion categories. The **Weekend Flash Sale** offers the highest average discount (**23K**), while **Festive Diwali** shows the lowest impact.
6.  **Operational Volume Tracking:** 
    *   Monitored a total of **3,510 unique orders** across the dataset.
7.  **Granular Data Exploration:** 
    *   Created a detailed **"Order Master"** table (Page 5) equipped with slicers for Customer Name, Product Name, and Promotion type for row-level auditing.
8.  **Geographical Sales Mapping:** 
    *   Visualized sales density across India, highlighting high-performance hubs in **Mumbai, Delhi, and Bangalore**.

---

## 🛠️ Technical Stack
*   **Power BI Desktop:** Core tool for development.
*   **Power Query (M):** Used for data cleaning, removing blanks from promotions, and formatting currency.
*   **DAX (Data Analysis Expressions):** 
    *   `Total Sales = SUM(Sales[Total Sales])`
    *   `Average Discount = AVERAGE(Sales[Total Discount])`
    *   Calculated measures for the side-by-side comparison visuals.
*   **Data Modeling:** Optimized a flat-file dataset into a reporting-ready structure.

---

## 🖼️ Dashboard Preview
> **Note:** To see the full interactivity, please download the `.pbix` file.

![Main Dashboard](https://github.com/charankumar08/Powerbi-projects/blob/main/Sales%20Analysis/Dashborad.pdf)  
*Figure 1: Executive Sales Overview & Geographical Distribution*

![Product Insights](https://github.com/charankumar08/Powerbi-projects/blob/main/Sales%20Analysis/Dashborad.pdf)  
*Figure 2: Top/Bottom Product Performance & Profitability*

---

## 📈 Key Insights from the Data
*   **The "Star" Product:** The **Apple iPhone 14** is the top performer, contributing **21.4M in Sales** and **2.14M in Profit**.
*   **Promotion Efficacy:** The **Weekend Flash Sale** is the most aggressive campaign, offering an average discount of **23K**.
*   **Sales Anomaly:** A significant drop-off in sales is noted moving into 2024, indicating a need for updated data or a shift in market strategy.
*   **Regional Strength:** Sales are heavily concentrated in Tier-1 Indian cities.

---

## 📂 Repository Contents
*   `Sales_Performance_Dashboard.pbix`: The source Power BI project.
*   `Resources/Sales_Data.csv`: The raw dataset used for analysis.
*   `Screenshots/`: A gallery of high-resolution images of each report page.

## 💡 How to Use
1.  Download the **`Sales_Performance_Dashboard.pbix`** file.
2.  Open it in **Power BI Desktop**.
3.  Use the **Date Filters** on Pages 3 and 4 to compare seasonal performance (e.g., comparing 2022 vs 2023).
4.  Filter by **Promotion Name** to see which discounts drive the most profit.

---
[⬅️ Back to Power BI Projects Portfolio](https://github.com/charankumar08/Powerbi-projects/tree/main)
