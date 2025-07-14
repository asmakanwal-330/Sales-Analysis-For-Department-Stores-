# Sales-Analysis-For-Department-Stores-

📊 Project Overview
This project involves analyzing historical weekly sales data from January 2011 to October 2012 for a chain of department stores. The goal was to:

i-Track overall sales trends

ii-Compare store and department performance

iii-Generate Year-over-Year (YoY) insights

iv-Allow for dynamic updates as new weekly data is added

📁 Datasets Used:
->Department.csv – Contains department names and IDs

->Stores.csv – Includes store locations and manager details

->All Data folder – Historical weekly sales from Jan 2011 to Oct 2012

->New Week folder – Sales for Oct 26, 2012 


⚙️ Key Steps:

🔄 Data Loading & Transformation
--> Used Power BI's "Get Data from Folder" to combine all historical weekly sales files.

-->Cleaned data in Power Query (e.g., removed unnecessary columns like Source.Name).

Renamed combined table to Sales.

📅 Calendar Table via DAX
-->Created a dynamic Calendar table using CALENDAR() DAX function.

-->Added derived column: Week of the Year.

🧠 Data Modeling
-->Designed a star schema with Sales as the fact table and Calendar, Stores, and Departments as dimensions.

📈 Dashboard Pages

1. Overall Sales Analysis
Includes:

-->Total sales across all stores

-->Number of departments and stores

-->Store-wise and department-wise sales performance

-->Weekly sales trend chart (with Year as legend)

-->YoY KPIs (Index & % Growth) in card visuals (across all data)

2. Week 20 Sales Analysis (YoY Comparison)  
Focused analysis on:
 --> Store 3, Department 1, Week 20 (this year vs last year)

 -->Bar chart showing sales comparison for Week 20 (YoY)

KPI cards:

📏 YoY Index = (Current Sales / Last Year Sales) × 100

📈 YoY % Growth = ((Current - Last Year) / Last Year) × 100

Used DAX time intelligence functions like SAMEPERIODLASTYEAR() to calculate YoY metrics


✅ Deliverables:
📁 Power BI (.pbix) file with two pages:

Overall Sales Analysis

Week 20 Sales Analysis

All visuals and metrics dynamically respond to updated data.















