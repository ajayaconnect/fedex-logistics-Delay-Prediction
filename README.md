# 🚚 FedEx Logistics Shipment Analysis (EDA)

## 📌 Project Overview
This project performs **Exploratory Data Analysis (EDA)** on a logistics shipment dataset based on a **FedEx business use-case**.  
The objective is to uncover the root causes of **delivery delays, rising logistics costs, and shipment profitability issues**.

This project simulates a real-world analytics workflow used in logistics and supply chain analytics.

---

## 🎯 Business Problem

A global logistics company has observed:

- 📈 Increase in delivery delays  
- 💰 Rising shipping and fuel costs  
- 📦 Declining profit per shipment  

Management wants to understand **why this is happening** and how data can help improve operations.

---

## 🧠 Project Objectives

- Perform data cleaning and preprocessing  
- Detect data quality issues (missing values, duplicates, outliers)  
- Analyze delivery performance and shipment trends  
- Identify cost drivers and loss-making shipments  
- Provide data-driven business recommendations  

---

## 📂 Dataset Description

The analysis uses **5 relational datasets**:

| Dataset | Description |
|---|---|
| Shipments | Shipment lifecycle, distance, cost, delivery status |
| Customers | Customer industry and location |
| Couriers | Courier vehicle type, rating and experience |
| Warehouses | Warehouse capacity and operations |
| Payments | Revenue, discount and payment details |

---

## 🧹 Data Cleaning & Preparation

During EDA, several real-world data issues were discovered and fixed:

- Removed duplicate shipment records  
- Handled missing pickup dates  
- Fixed invalid date records (delivery before pickup)  
- Corrected negative delay values  
- Treated outliers in shipment distance and weight  
- Standardized data types and formats  

This ensured **reliable and accurate analysis**.

---

## 📊 Exploratory Analysis

### 🚚 Delivery Performance Insights
- Road transport showed **higher delay risk** than air shipments  
- Long-distance shipments had **longer delivery times**  
- Some regions consistently experienced **higher delay rates**

### 💰 Cost & Profitability Insights
- Strong correlation between **distance, fuel cost and shipping cost**  
- Identified shipments where **cost exceeded revenue**  
- Heavy shipments significantly increased logistics cost

### 🏭 Operational Insights
- Vendor/courier performance influenced delivery delays  
- Warehouse load and shipment mode affected delivery efficiency

---

## 📈 Business Impact

The analysis shows the company can improve operations by:

- Choosing shipment modes strategically  
- Monitoring vendor performance using KPIs & SLAs  
- Strengthening logistics in high-delay regions  
- Reducing shipment weight through packaging optimization  

---

## 📌 Strategic Recommendations

### Smart Shipment Strategy
- ✈️ Air → Urgent & high-priority shipments  
- 🚢 Ocean → Bulk shipments  
- 🚚 Road → Regional deliveries  

### Vendor Performance Management
- Introduce vendor performance KPIs  
- Audit consistently delayed vendors  

### Regional Logistics Improvement
- Improve last-mile delivery in high-delay regions  
- Optimize customs and clearance processes  

### Cost Optimization
- Consolidate shipments  
- Reduce packaging weight to cut shipping cost  

---

## 🛠️ Tools & Technologies
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## 📌 Project Outcome

This EDA project demonstrates how data analytics can help logistics companies:

- Reduce delivery delays  
- Improve operational efficiency  
- Optimize shipping costs  
- Support data-driven decision making  

---

⭐ If you found this project useful, feel free to star the repository!
