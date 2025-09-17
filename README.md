
## 📌 Project Overview

Effective inventory and sales management are critical for profitability in the **retail and wholesale industry**. This project analyzes **vendor performance** to identify underperforming brands, top vendors, bulk purchasing impact, inventory turnover, and profitability trends.

Using **SQL, Python (Pandas, Seaborn, Matplotlib), Jupyter Notebook, and Power BI**, I built an **end-to-end analytics pipeline** to transform raw datasets into actionable business insights and dashboards.

---
## 🎯 Business Problem

The project aims to answer key business questions:

- Which vendors contribute the most to **sales and gross profit**?

- Which brands are **underperforming** and may need **promotional or pricing adjustments**?

- How does bulk **purchasing impact unit costs**?

- What is the **inventory turnover rate** and how can it reduce holding costs?

- How does **profitability vary across high vs. low performing vendors**?
## 🚀 Project Workflow

1.) **Data Collection** → Combined 6 raw CSVs into SQLite database.

2.) **Data Preparation** → Extracted relevant columns → Created vendor_sales_summary.csv.

3.) **Data Cleaning & EDA** → Pandas, Seaborn, Matplotlib for filtering, visualization, and correlation analysis.

4.) **Business Analysis** → Vendor profitability, sales-to-purchase ratio, bulk cost impact, seasonal trends.

5.) **Dashboard Creation** → Power BI for vendor contribution, brand performance, low performing vendors/brands.
## 🗂 Dataset Description

The project integrates 6 raw CSV datasets:

1.) **Vendor_invoice** → Vendor transactions with invoice details.

2.) **Sales** → Sales data with quantities, prices, vendors, and brands.

3.) **Purchase_prices** → Purchase cost details per brand/vendor.

4.) **Purchases** → Purchase order, receiving, and invoice data.

5.) **End_inventory** → Closing inventory details by store.

6.) **Begin_inventory** → Opening inventory details by store.

After cleaning and merging, the consolidated dataset "vendor_sales_summary.csv" was created with **18 columns and 10,692 rows** (reduced to 8,564 rows after cleaning).


**Key Columns in vendor_sales_summary:**
VendorNumber, VendorName, Brand, PurchasePrice, ActualPrice, Volume, TotalPurchaseQuantity, TotalPurchaseDollars, TotalSalesQuantity, TotalSalesDollars, GrossProfit, ProfitMargin, StockTurnover, SalesToPurchaseRatio, FreightCost
## 🛠️ Tech Stack

- **SQL (SQLite)** → Data integration & querying.

- **Python (Pandas, NumPy, Scipy, Matplotlib, Seaborn)** → Data cleaning, EDA, correlation & statistical analysis.

- **Jupyter Notebook** → Interactive data analysis & visualization.

- **Power BI** → Dashboard creation for vendor & brand performance insights.
## 🔎 Data Cleaning & EDA
- **Summary Statistics:**
  ![image alt](https://github.com/Kaif2596/vendor-Performance-Data-Analysis/blob/main/image1.png)
  
- Removed **negative/zero profit margins and sales** to ensure consistent data quality
  ![image alt](https://github.com/Kaif2596/vendor-Performance-Data-Analysis/blob/main/image2.png)

- Reduced dataset from **10,692 rows → 8,564 quality rows** after filtering.
  ![image alt](https://github.com/Kaif2596/vendor-Performance-Data-Analysis/blob/main/image4.png)

- Outlier detection with boxplots and descriptive statistics.
  ![image alt](https://github.com/Kaif2596/vendor-Performance-Data-Analysis/blob/main/image3.png)

- Correlation heatmap showed:
  ![image alt](https://github.com/Kaif2596/vendor-Performance-Data-Analysis/blob/main/image5.png)

  - **0.999 correlation** between purchase and sales quantity → efficient inventory flow.

  -  correlation (-0.179) between profit margin and sales price → competitive pricing pressures.

- Freight cost variance ranged from **$0.09 → $257,000**, indicating logistics inefficiencies.
## 📈 Key Insights

- Identified **brands with low sales but high profit margins**, useful for promotions.

- Highlighted **low performing vendors** despite large purchase volumes.

- Confirmed **bulk purchase discounts** lowering unit costs.

- Assessed **inventory turnover** for fast vs. slow-moving products.

- Seasonal analysis revealed vendor/brand demand patterns.
## 📊 Power BI Dashboard

The interactive Vendor Performance Dashboard tracks key KPIs:

- **$441M** Total Sales

- **$307M** Total Purchases

- **$134M** Gross Profit

- **39%** Profit Margin

- **$3M** Unsold Capital

Visuals include:

- Purchase Contribution % (Pie Chart)

- Top Vendors by Sales (Bar Chart)

- Top Brands by Sales (Bar Chart)

- Low Performing Vendors (Bar Chart)

- Low Performing Brands (Scatter Plot with Profit Margin vs. Sales)
## 📈 Results & Impact

-  a **robust vendor analytics pipeline** to support procurement and pricing strategies.

- Enabled **data-driven decisions** in vendor negotiations, promotions, and inventory optimization.

- Delivered dashboards that provide **real-time visibility into $441M sales and $134M gross profit performance.**

## 📂 Repository Structure

├── data/  
│   ├── vendor_invoice.csv  
│   ├── sales.csv  
│   ├── purchase_prices.csv  
│   ├── purchases.csv  
│   ├── end_inventory.csv  
│   ├── begin_inventory.csv  
│   └── vendor_sales_summary.csv  
├── notebooks/  
│   └── vendor_performance_analysis.ipynb  
├── dashboard/  
│   └── vendor_performance_dashboard.pbix  
├── images/  
│   └── dashboard_screenshot.png  
├── README.md  

## 🔮 Future Improvements

- Add **forecasting models (ARIMA/Prophet)**for vendor/brand sales prediction.

- Incorporate **vendor delivery reliability metrics** (On-Time Delivery %).

- Automate **ETL pipeline** for real-time Power BI updates.
## 👨‍💻 Author

- Name: Mohd Kaif Ansari

- 💼 Aspiring Data Analyst | AI & Data Science Enthusiast

- Contact : 9354578826

- Email : kaifansari1808@gmail.com

- LinkedIn : https://www.linkedin.com/in/mohd-kaif-ansari-4a93aa31b/


---
