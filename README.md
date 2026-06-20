# Coffee Sales Performance Dashboard

An end-to-end Excel data analytics project that processes raw transactional data to build an interactive, production-ready business intelligence dashboard. 

📊 **[Interact with the Live Excel Dashboard Here](PASTE_YOUR_ONEDRIVE_SHARE_LINK_HERE)** *(Note: Replace this placeholder text with your actual OneDrive share link!)*

---

## 📌 Project Overview
This project demonstrates the full data lifecycle—from raw data ingestion to final stakeholder presentation. The goal was to analyze coffee sales performance over time, identify high-value geographic markets, and isolate top-tier customers to drive strategic business decisions.

### Key Insights Delivered:
* **Total Sales Over Time:** A granular timeline analysis tracking revenue fluctuations across coffee types (Arabica, Excelsa, Liberica, Robusta).
* **Sales by Country:** A geographic breakdown highlighting market dominance between the United States, United Kingdom, and Ireland.
* **Top 5 Customers:** A loyalty and volume-based ranking identifying the highest-spending clients to assist targeted marketing campaigns.

---

## 📂 Dataset Architecture
The project architecture is built on three core relational data sheets combined into a unified model:
1. `orders`: Main transaction log tracking order dates, product IDs, customer IDs, and quantities.
2. `customers`: Customer profiles containing names, email addresses, geographic locations, and loyalty card status.
3. `products`: Product catalog detail including coffee roast types (Dark, Medium, Light), packaging sizes (0.2kg to 2.5kg), unit prices, and profit margins.

---

## 🛠️ Data Processing & Methodology

### 1. Data Cleaning & Integration
* Standardized date formats and eliminated duplicates across all sheets.
* Utilized lookup formulas (`XLOOKUP`/`VLOOKUP`) to dynamically pull customer demographics and product specifications directly into the `orders` sheet, creating a master data table.

### 2. Aggregation via Pivot Tables
* Generated dynamic summary tables on dedicated sheets (`totalSales`, `countryBarChart`, `topCustomers`) to calculate metrics without altering the core database.

### 3. Dashboard UI & Interactive Features
* Built a cohesive, custom-themed visual interface on the `dashboard` worksheet.
* Integrated **interactive multi-select Slicers** (*Order Date*, *Roast Type Name*, *Size*, and *Loyalty Card Status*) linked globally across all charts to enable dynamic cross-filtering.

---

## 🖥️ Dashboard Preview
*(Tip: You can take a screenshot of your Excel screen, save it as `dashboard.png` in your GitHub repository, and display it here using the markdown line below!)*
![Coffee Sales Dashboard Preview](dashboard.png)

---

## 🚀 How to Use the Repository
1. **Clone or Download:** Download the `.xlsx` file from this repository.
2. **Interact Online:** Click the live project link at the top of this file to interact with the dashboard via Excel Web App without needing an Excel license.
3. **Explore Filters:** Use the Slicer panel on the right side of the dashboard to slice data by package size or roast preference to see charts update in real-time.
