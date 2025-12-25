# 📦 Purchasing Performance Dashboard (Power BI)

## 📌 Project Description
This project analyzes **purchasing and procurement data** using Power BI to evaluate supplier performance, purchasing spend, delivery efficiency, and order execution quality.  
The dashboard is designed to support procurement and operations teams in monitoring key metrics and making data-driven decisions to optimize cost control, vendor management, and delivery performance.



## 🧠 Business Context
Procurement operations often face challenges such as:
- Increasing purchasing costs
- Dependency on a limited number of vendors
- Late or rejected orders impacting operations
- Lack of visibility at both order-level and line-item-level data

This project addresses these challenges by combining **order-level** and **transaction-level** purchasing data into a unified analytics solution.



## 🗂️ Data Model (Star Schema)

The data model follows a **star schema** design with **two fact tables**, enabling both high-level and detailed procurement analysis.

### ⭐ Fact Tables

#### 1. Fact_PurchaseOrderHeader
Order-level information including:
- Purchase Order ID
- Order Date, Due Date, Ship Date
- Vendor ID, Ship Method ID
- Order Status (Complete, Pending, Rejected, Approved)
- Freight Cost and Tax Amount
- On-time delivery indicators

Supports **delivery performance, lead time, and vendor-level analysis**.

#### 2. Fact_PurchaseOrderDetail
Line-item-level purchasing data including:
- Purchase Order ID
- Product ID
- Order Quantity
- Unit Price
- Line Total (actual purchase cost)

Supports **spend analysis, product-level insights, and cost breakdowns**.

### 📐 Dimension Tables
- **Dim_Vendor**
- **Dim_Product**
- **Dim_ProductCategory**
- **Dim_ProductSubcategory**
- **Dim_ShipMethod**
- **Date**



## 📊 Key Metrics
- **Total Cost**
- **Total Purchase Orders**
- **On-Time Delivery Rate (%)**
- **Average Unit Price**
- **Average Lead Time**
- **Rejected / Pending Order Rate**
- **Vendor Active Rate**



## 📊 Key Insights & Visualizations

### 🔍 Dashboard Preview
The project includes four main dashboards: **Overview**, **Vendors**, **Orders**, and **Transaction**.



### 1️⃣ Dashboard 1: Purchasing Overview
![image alt](https://github.com/tranthuyquynh122-cyber/Purchasing-Dashboard/blob/1b1f1cb89018f35dd9091d06e3383abbda478a24/Screenshot%202025-12-24%20235115.png)

#### 🔎 Observation
- Total purchasing cost and total orders increased significantly compared to the previous year.
- Purchase spend is heavily concentrated in **Components** and **Other** categories.
- Average unit price remains stable, while lead time fluctuates slightly over time.

#### 💡 Recommendation
- Monitor high-spend categories closely to identify negotiation or cost optimization opportunities.
- Track lead time trends to mitigate supply chain risks.



### 2️⃣ Dashboard 2: Vendor Performance
![image alt](https://github.com/tranthuyquynh122-cyber/Purchasing-Dashboard/blob/1b1f1cb89018f35dd9091d06e3383abbda478a24/Screenshot%202025-12-24%20235128.png)

#### 🔎 Observation
- A small group of vendors accounts for a large proportion of total purchasing cost.
- Vendors with higher rejection or defect rates often show higher costs and longer lead times.
- Most vendors maintain high on-time delivery, but a few underperformers impact overall efficiency.

#### 💡 Recommendation
- Reduce dependency on high-risk vendors by diversifying suppliers.
- Use vendor KPIs to guide preferred vendor selection and contract evaluation.



### 3️⃣ Dashboard 3: Orders Performance
![image alt](https://github.com/tranthuyquynh122-cyber/Purchasing-Dashboard/blob/1b1f1cb89018f35dd9091d06e3383abbda478a24/Screenshot%202025-12-24%20235145.png)

#### 🔎 Observation
- Most purchase orders are completed successfully, but rejected and pending orders still represent operational risk.
- On-time delivery varies by month, indicating seasonal or capacity-related challenges.
- Freight cost differs significantly by shipping method.

#### 💡 Recommendation
- Investigate causes of rejected and pending orders to improve process efficiency.
- Optimize shipping methods by balancing freight cost and delivery reliability.



### 4️⃣ Dashboard 4: Transaction-Level Analysis
![image alt](https://github.com/tranthuyquynh122-cyber/Purchasing-Dashboard/blob/1b1f1cb89018f35dd9091d06e3383abbda478a24/Screenshot%202025-12-24%20235153.png)

#### 🔎 Observation
- Transaction-level analysis reveals variations in unit price and order quantity across vendors.
- Repeated delayed or rejected transactions are observed for certain vendors.
- Line-level data highlights cost drivers not visible at order summary level.

#### 💡 Recommendation
- Implement transaction-level monitoring to detect issues early.
- Strengthen approval and validation processes for high-risk vendors.



## 🔍 Final Conclusion & Recommendations

👉 Based on the insights across all dashboards, the purchasing analysis highlights the need to balance **cost efficiency**, **vendor reliability**, and **delivery performance**.

### 📌 Key Takeaways
- Purchasing spend and order volume are increasing, raising cost and dependency risks.
- Vendor performance varies significantly and directly impacts operational efficiency.
- Transaction-level data provides critical insight into hidden cost drivers.

### 📌 Recommendations
- Establish a balanced procurement KPI framework covering cost, delivery, and reliability.
- Actively manage vendor relationships using performance-based metrics.
- Leverage detailed transaction data to support proactive procurement planning.



