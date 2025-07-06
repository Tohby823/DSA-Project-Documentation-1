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

- **SQL Server** [Download Here](https://learn.microsoft.com/en-us/ssms/install/install)
  – For data querying and insight extraction  
- **Microsoft Excel** [Download Here](httpa://microsoftexcel.com)
  – For preliminary data inspection  
- **GitHub** [Download Here](https://github.com)
  – For documentation and portfolio hosting

---

### Case Scenario I – Sales & Shipping Insights

### 1. Product Category with the Highest Sales  
 *TECHNOLOGY* – Total sale: *89061.050*

### 2. Top 3 and Bottom 3 Regions by Sales  
Top 3:
|Region| Sales|
|-------|------|
|Atlantic|  89061.050|
|Quebec|  45923.760|
|Prarie|  41343.210|

Bottom 3:  
|Region| Sales|
|-------|------|
|West | 2.240|
|West | 3.200|
| Yukon | 3.230|

### 3. Total Sales of Appliances in Ontario  
 *202346.840*

### 4. Recommendation to Increase Revenue from Bottom 10 Customers 

*Bottom 10 Customers and the revenue generated*
|Customer_Name| Sales|
|--------------|-----|
|Ricardo Emerson |2.240|
| Ken Dana |3.200|
| Benjamin Patterson |	3.230|
| Adam Hart |	3.410|
| Andy Reiter |	3.420|
| Maria Bertelson |3.630|
| Katrina Bavinger |	3.770|
|Adam Hart |	3.850|
| Jeremy Farry | 3.960|
| Don Weiss |	4.940|
  
 *To increase revenue from the bottom 10 customers, I recommend implementing targeted promotions based on their previous purchase history and offering personalized discounts to re-engage them. Additionally, bundling low-interest items with popular products can increase order value. It's also important to collect feedback from these customers to understand pain points that might be limiting their spending.*

### 5. Shipping Method with the Highest Cost  
 *Delivery Truck* – Total cost: *164.730*

---

### Case Scenario II – Customer Value & Profitability

### 6. Most Valuable Customers and What They Buy  
|S/N|	Customer_Name| Product_Category|	Product_Sub_Category|	Sales|
|--|-------------|----------------|---------------------|-------|
|1| Emily Phan|	Technology|	Office Machines|	89061.050|
|2	|Jasper Cacioppo|	Technology|	Office Machines|	45923.760|
|3|	Craig Carreira|	Technology|	Office Machines|	41343.210|
|4|	Dennis Kane|	Technology|	Copiers and Fax|	33367.850|
|5	|Karen Carlisle|	Technology|	Copiers and Fax|	29884.600|

### 7. Small Business Customer with the Highest Sales  
 |	Customer_Name|Customer_Segment|Sales|
 |---------------|-----------------|-----|
 |Dennis Kane| Small Business|33367.850|

### 8. Corporate Customer with the Most Orders  
|	Customer_Name|Customer_Segment|Order_Quantity|
 |---------------|-----------------|-----|
 |Sonia Cooley| Corporate|50|

### 9. Most Profitable Consumer Customer  
|	Customer_Name|Profit|
 |---------------|-----|
 |Emily Phan| 27220.690|

### 10. Customers Who Returned Items and Their Segment   
While the dataset does not explicitly track returned items, I used negative profit values as a proxy to identify customers likely associated with returns or loss-making orders.

A total of 308 customers recorded negative profit, which could indicate returns, over-discounts, or shipping-related losses. These customers were found across all three segments—Consumer, Corporate, and Small Business—with a noticeable concentration in the Consumer segment.

| **Customer_Name** | **Customer_Segment** | **Profit** |
| ------------------ | --------------------- | ---------- |
| Jamie Frazer       | Small Business        | -473.720   |
| Benjamin Patterson | Corporate             | -1964.760  |
| Sylvia Foulston    | Home Office           | -1302.760  |
| Anemone Ratner     | Small Business        | -57.200    |
| Troy Staebel       | Small Business        | -916.200   |
| Bryan Davis        | Corporate             | -328.180   |
| Maribeth Yedwab    | Home Office           | -1109.550  |
| Joni Sundaresam    | Home Office           | -146.620   |
| Scot Coram         | Corporate             | -951.780   |
| Max Engle          | Corporate             | -1668.500  |
| Alan Haines        | Home Office           | -1401.170  |
| Neoma Murray       | Small Business        | -697.180   |
| Sarah Jordon       | Consumer              | -798.310   |
| Brad Eason         | Small Business        | -473.360   |
| Julia West         | Home Office           | -13057.200 |
| Dennis Pardue      | Corporate             | -1207.430  |
| Greg Guthrie       | Corporate             | -1462.990  |
| Theone Pippenger   | Corporate             | -1400.140  |
| Fred Harton        | Home Office           | -71.540    |
| Doug Bickford      | Corporate             | -666.930   |
| Hunter Glantz      | Corporate             | -188.570   |
| Mick Hernandez     | Home Office           | -347.070   |
| Quincy Jones       | Corporate             | -82.080    |
| Joe Elijah         | Home Office           | -324.020   |
| Irene Maddox       | Consumer              | -6240.160  |

The rest of the table is in an excel sheet uploaded to this repository


### 11. Shipping Cost Appropriateness Based on Order Priority  
 | Ship_Mode          | Order_Priority | Num_Orders | Avg_Shipping Cost |
| ------------------ | -------------- | ------ | ------------------ |
| **Delivery Truck** | Critical       | 228    | 47.30             |
| **Delivery Truck** | High           | 248    | 45.19             |
| **Delivery Truck** | Low            | 250    | 44.53             |
| **Delivery Truck** | Medium         | 205    | 46.15             |
| **Delivery Truck** | Not Specified  | 215    | 43.67             |
| **Express Air**    | Critical       | 200    | 8.71              |
| **Express Air**    | High           | 212    | 6.86              |
| **Express Air**    | Low            | 190    | 8.17              |
| **Express Air**    | Medium         | 201    | 8.13              |
| **Express Air**    | Not Specified  | 180    | 8.17              |

After analyzing the shipping cost data across order priorities, it was observed that both Delivery Truck and Express Air were used for all priority levels, including Critical and Low. This reflects a lack of alignment between shipping method and urgency.

Surprisingly, the average shipping cost for Express Air is significantly lower (6.86–8.71) compared to Delivery Truck (43.67–47.30), which is unexpected since Express Air is typically more expensive.

Based on this, two key issues emerge:

- There may be inconsistencies in how shipping costs were recorded.
- KMS may not be strategically assigning shipping methods based on order priority.

---

### Data Analysis
### SQL Techniques Used

- `GROUP BY`, `ORDER BY`, `LIMIT`  
- Aggregates: `SUM()`, `COUNT()`, `AVG()`, `MAX()`  
- `CASE WHEN` for conditional analysis  
- Filtering: `WHERE`, `IN`, `BETWEEN`  


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
