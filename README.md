🍕 Pizza Sales Dashboard – Power BI :

An interactive Power BI dashboard that delivers comprehensive insights into pizza sales performance across different stores, regions, and time periods. This project highlights data cleaning in Power Query, advanced DAX measures, and dynamic visualizations designed for restaurant managers and stakeholders to optimize menu offerings, marketing strategies, and inventory planning.

📊 Project Overview :

The pizza business thrives on understanding which products, locations, and time windows drive the most revenue and profit. This dashboard was created to:

Track sales trends by day, week, month, and region

Identify top-selling pizza varieties (units sold and revenue)

Monitor key financial metrics such as total revenue, total profit, average order value, and profit margins

Enable interactive filtering for drill-down analysis by store location, pizza category (e.g., vegetarian, non-vegetarian), and time frame

By combining cleaned pizza sales data with tailored measures, this dashboard helps answer questions like “Which store generated the highest profit last month?” or “How did promotional pricing affect average order value?”

🧰 Tools & Technologies :
Power BI Desktop


Data modeling, interactive report creation, and visualization

Power Query Editor

Data cleaning, transformation, table merging, and applied steps documentation

DAX (Data Analysis Expressions)

Custom measures and KPIs for sales, profit, and growth rates

Source Files

pizza sales.pbix – Power BI project file containing data model and report


🧹 Data Cleaning & Preparation :

All data preparation was performed in Power Query Editor before building visuals:

Import & Combine Data

Loaded raw pizza sales data (e.g., separate tables for Orders, Menu Items, Stores).

Used Merge Queries to join Orders and Menu Items on ItemID and Append Queries if multiple monthly files existed.

Remove Duplicates & Nulls

Filtered out duplicate transactions based on OrderID.

Removed rows where critical fields (e.g., OrderDate, StoreID, Quantity, or Revenue) were null or zero.

Standardize Product & Store Names

Trimmed whitespace and corrected inconsistent naming (e.g., “Margherita” vs. “margherita”).

Converted all text columns to Proper Case for uniformity.

Date & Time Transformations

Converted OrderDateTime to proper Date/Time data type.

Extracted separate Year, Month, Day of Week, and Hour columns for time-based analysis.

Calculated Columns

Created a Profit column:

ini
Copy
Edit
Profit = Revenue – Cost  
Added a OrderCategory column based on Quantity thresholds (e.g., “Single”, “Family Pack”, “Party Order”).

Data Type Corrections

Ensured numeric fields (Quantity, Revenue, Cost) are set to Decimal or Whole Number.

Set StoreID and ItemID as text to prevent type mismatches during joins.

📈 Key Features & Visuals :

Sales Trend Analysis

Line Chart showing daily/weekly/monthly revenue and profit.

Slicers for selecting specific date ranges (e.g., last 7 days, last 6 months).

Top Products & Categories

Bar Chart ranking top 10 pizza varieties by units sold.

Treemap visualizing revenue contribution by category (e.g., Veg, Non-Veg, Specialty).

Regional & Store Performance

Map Visual plotting store locations with color-coded revenue/profit bubbles.

Matrix/Table view showing each store’s metrics: total orders, average ticket size, total profit.

KPI Cards

Total Revenue, Total Profit, Average Order Value, Total Orders displayed as KPI cards for quick glance.

Profitability Analysis

Scatter Chart comparing Average Order Value vs. Profit Margin for each store, identifying high-value locations.

Pie Chart breakdown of profit share by pizza category.

Interactive Filtering & Drill-Through

Slicers for Store, Item Category, Date.

Drill-through capability: click on a store’s data point to view store-level details (orders, peak hours, best-selling items).

📂 Files Included :
pizza sales.pbix

Power BI Desktop file containing the full data model, queries, DAX measures, and report pages.


📸 Dashboard Preview :

![Screenshot (791)](https://github.com/user-attachments/assets/a24d9d5f-6409-4b74-853d-01b4702960f1)



Line chart showing monthly revenue and profit trends.


Bar chart highlighting top 10 pizza varieties.


Map visual displaying store locations sized by revenue.

🔧 How to Use This Dashboard :

Download & Open

Download pizza sales.pbix from the repository.

Open in Power BI Desktop (version 2.XX or higher recommended).


If a separate data file (e.g., pizza-sales-data.xlsx) is included, ensure it’s placed in the same folder as the .pbix.

In Power BI Desktop, go to Home → Transform data → Data source settings and update the file path if necessary.

Interact with Filters

Use slicers on the report pages to filter by Date, Store, and Item Category.

Click on any data point to drill through to details (e.g., store-level breakdown).

Export or Publish

Export visuals as PNG/PDF for presentations.


📬 Contact :
Ayush Gupta

📍 New Delhi, India

📧 ayushgupta22294@gmail.com

🔗 LinkedIn

🔗 https://github.com/ayush-g1

Feel free to reach out if you have any questions, feedback, or collaboration ideas!

⭐ Notes
This is a self-initiated portfolio project showcasing data analytics and visualization skills—no real company data was used.

All transformations, DAX calculations, and visual designs were implemented personally to demonstrate proficiency in Power BI.

Screenshot images are for illustrative purposes; actual metrics may vary based on the source dataset.

Thank you for reviewing my Pizza Sales Dashboard project. I appreciate your time and welcome any suggestions or opportunities to collaborate.
