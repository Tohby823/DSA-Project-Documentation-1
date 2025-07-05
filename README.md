# DSA-Project-Documentation-1

SQL-based analysis of inventory, customer, and shipping data for Kultra Mega Stores (2009–2012) to uncover insights on sales, profitability, and delivery efficiency.

## Kultra Mega Stores SQL Case Study | DSA Capstone Project

This project is part of the Data Analysis Capstone from the **DSA Program**, involving the use of SQL to analyze historical order and shipping data from **Kultra Mega Stores (KMS)**. The objective is to uncover patterns in sales performance, customer value, shipping efficiency, and regional trends to support business decisions for KMS’s Abuja division.

--- 

### Project Overview

### Company Background

Kultra Mega Stores, headquartered in Lagos, provides office supplies and furniture to consumers, small businesses, and large corporations across Nigeria. The Abuja branch requires actionable insights to increase revenue, improve customer retention, and optimize shipping.

---

### Data Source

- **Source**: Excel file provided via DSA Capstone Project Files
- **Time Frame**: 2009–2012  
- **Data Categories**: Orders, Products, Customers, Shipping Details  

---

### Tools Used

- **SQL (PostgreSQL / MySQL)** – For data querying and insight extraction  
- **Microsoft Excel** – For preliminary data inspection  
- **GitHub** – For documentation and portfolio hosting

---

### Case Scenario I – Sales & Shipping Insights

### 1. Product Category with the Highest Sales  
 *TECHNOLOGY* – Total sale: *89061.050*

### 2. Top 3 and Bottom 3 Regions by Sales  
Top 3:  
- Atlantic  – Total sale: *89061.050*
- Quebec  – Total sale: *45923.760*
- Prarie  – Total sale: *41343.210*

Bottom 3:  
- West  – Total sale: *2.240*
- West  – Total sale: *3.200*
- Yukon  – Total sale: *3.230*

### 3. Total Sales of Appliances in Ontario  
 *202346.840*

### 4. Recommendation to Increase Revenue from Bottom 10 Customers 

*Bottom 10 Customers and the revenue generated*
- Ricardo Emerson -	2.240
- Ken Dana - 3.200
- Benjamin Patterson -	3.230
- Adam Hart -	3.410
- Andy Reiter -	3.420
- Maria Bertelson -	3.630
- Katrina Bavinger -	3.770
- Adam Hart -	3.850
- Jeremy Farry -	3.960
- Don Weiss -	4.940
  
 *To increase revenue from the bottom 10 customers, I recommend implementing targeted promotions based on their previous purchase history and offering personalized discounts to re-engage them. Additionally, bundling low-interest items with popular products can increase order value. It's also important to collect feedback from these customers to understand pain points that might be limiting their spending.*

### 5. Shipping Method with the Highest Cost  
 *Delivery Truck* – Total cost: *164.730*

---

### Case Scenario II – Customer Value & Profitability

### 6. Most Valuable Customers and What They Buy  
 *[Top 3 customers with frequent purchases – and categories]*

### 7. Small Business Customer with the Highest Sales  
 *[Customer Name]* – *[Insert value]*

### 8. Corporate Customer with the Most Orders  
 *[Customer Name]* – *[Insert number of orders]*

### 9. Most Profitable Consumer Customer  
 *[Customer Name]* – Profit: *[Insert value]*

### 10. Customers Who Returned Items and Their Segment  
 *[List customers and their segment]*

### 11. Shipping Cost Appropriateness Based on Order Priority  
 *[Explain whether Express Air or Truck delivery matched the order priority in high/low urgency cases]*

---

### SQL Techniques Used

- `GROUP BY`, `ORDER BY`, `LIMIT`  
- Aggregates: `SUM()`, `COUNT()`, `AVG()`, `MAX()`  
- `CASE WHEN` for conditional analysis  
- Filtering: `WHERE`, `IN`, `BETWEEN`  
- Joins across orders, customers, and shipping tables

---

## 📈 Business Insights Summary

- Top-selling product categories and high-performing regions identified  
- Shipping costs need realignment with priority levels to reduce inefficiency  
- Targeting underperforming customers and regions can boost revenue  
- Customer segmentation reveals key opportunities for tailored marketing

---

##  Next Steps

- Visualize customer and sales trends using Power BI  
- Add seasonality and time-based trend analysis  
- Create a dashboard summary for business managers

---

## Folder Structure (Optional)

```bash sql-kultra-mega-stores
├── queries/
│   ├── case_scenario_1.sql
│   └── case_scenario_2.sql
├── README.md
├── results/
│   ├── top_customers.csv
│   └── shipping_costs.csv
└── dataset/
    └── KMS_orders_2009_2012.xlsx
