# 📌 E-Commerce Analytics Dashboard | Power BI

## 📌 Project Overview
This project is an **end-to-end E-Commerce Analytics solution built in Power BI**.  
It converts large-scale transactional data into **actionable business insights** across sales, profitability, marketing, operations, and customer behavior.

The dashboard suite is designed for **executives, finance, marketing, operations, and customer experience teams**, following real-world enterprise analytics practices.

---

## 📌 Business Problem
The business operates across **multiple sales channels (Web, App, Marketplace, Affiliate, Social)** and **multiple regions (India, APAC, EMEA, AMER)**.

Despite high transaction volume, leadership faced challenges such as:
- Lack of clarity on **profitable channels**
- Inefficient **marketing spend**
- Poor visibility into **delivery SLA performance**
- High **return rates without clear reasons**
- Flat dashboards due to **large, evenly distributed data**

---

## 📌 Project Objectives
- Build a **single source of truth** using Power BI
- Provide **role-based dashboards** for different stakeholders
- Analyze **revenue, profit, marketing ROI, operations, and customer behavior**
- Preserve raw data accuracy while surfacing **meaningful insights**
- Apply **industry best practices** in data modeling, DAX, and dashboard design

---

## 📌 Dataset Information
- **FactSales_200k.csv** → 200,000+ transaction records
- **FactMarketingSpend.csv** → Marketing spend and clicks
- **Dimension Tables** → Date, Channel, Region, Customer

⚠️ Note:  
All datasets are **synthetic and created for learning/demo purposes only**.

---

## 📌 Data Modeling
- **Star Schema** design
- Central fact tables with supporting dimensions
- Single-direction relationships
- Dedicated **Measures Table** for DAX
- Optimized for performance and scalability

---

## 📌 Key Metrics & KPIs
### Sales & Finance
- Net Revenue
- Gross Profit
- Gross Margin %
- Average Order Value (AOV)
- Total Orders
- Units Sold

### Marketing
- Marketing Spend
- Customers Acquired
- CAC (Customer Acquisition Cost)
- ROAS (Return on Ad Spend)

### Operations & Customer Experience
- On-Time Delivery %
- Returned Orders
- Return Rate %
- Shipping Cost

### Time Intelligence
- Revenue YTD
- Revenue MTD
- Revenue YoY %

---

## 📌 Dashboards Created (5 Pages)

### 1️⃣ Executive Overview
**Audience:** CEO / Leadership  
**Purpose:** High-level business health monitoring  
**Insights:** Revenue growth, profitability, AOV, returns, SLA performance

---

### 2️⃣ Sales & Profit Analysis
**Audience:** Finance & Sales teams  
**Purpose:** Understand revenue vs profitability  
**Insights:** Margin leakage, discount impact, value vs volume analysis

---

### 3️⃣ Marketing Performance
**Audience:** Marketing & Growth teams  
**Purpose:** Evaluate marketing efficiency  
**Insights:** CAC, ROAS, spend vs revenue, customer acquisition by channel

---

### 4️⃣ Operations & SLA
**Audience:** Operations & Logistics teams  
**Purpose:** Monitor delivery performance  
**Insights:** SLA adherence, shipping cost by region, return drivers

---

### 5️⃣ Customer & Returns
**Audience:** Customer Experience & Product teams  
**Purpose:** Understand customer quality and dissatisfaction  
**Insights:** AOV by channel, return rate, payment method behavior, return reasons

---

## 📌 Key Analytical Challenge & Solution
### Challenge
Due to the **large and evenly distributed dataset**, raw aggregations resulted in **flat bar charts**, making insights visually weak.

### Solution
A **two-layer analytics approach** was implemented:
- **Truth Layer:** Original measures for KPI accuracy
- **Insight Layer:** Weighted measures at the DAX level to highlight meaningful business differences

✔ Raw data, schema, and relationships were **not modified**  
✔ Weighting was applied **only for comparative visuals**

---

## 📌 Advanced DAX Techniques Used
- Time intelligence (YTD, MTD, YoY)
- Ratio-based KPIs (Margin %, ROAS, CAC)
- Conditional logic using `SWITCH`
- Analytical weighting using helper measures
- Separation of truth vs insight metrics

(See `Key_DAX_Measures.md` for full DAX reference)

---

## 📌 Dashboard Design Principles
- Clean white/light background
- Consistent color theme
- Green for positive KPIs, red for risk indicators
- Minimal borders and clutter
- Executive-friendly layout
- Consistent slicers across pages

---

## 📌 Tools & Technologies
- Power BI Desktop
- Power Query
- DAX
- CSV (synthetic data)
- GitHub for documentation & versioning

---

## 📌 How to Use
1. Download the `.pbix` file
2. Open in Power BI Desktop
3. Refresh data if required
4. Explore dashboards using slicers and filters

---

## 📌 Key Learnings
- Enterprise-style data modeling
- Advanced DAX for business analytics
- Handling large datasets with evenly distributed data
- Designing executive-ready dashboards
- Separating **data accuracy** from **analytical insight**

---

## 📌 Interview-Ready Summary
> “I built an enterprise-style Power BI e-commerce analytics solution using a star schema and advanced DAX.  
> The project delivers five role-based dashboards covering sales, profit, marketing ROI, operations, and customer behavior.  
> To handle large evenly distributed data, I preserved raw KPIs for accuracy and applied analytical weighting at the DAX layer to surface meaningful insights without altering the underlying dataset.”

---

## 📌 Project Structure
Ecommerce-PowerBI-Analytics/
│
├── 📌 Dashboards/
│   ├── Executive_Overview.png
│   ├── Sales_Profit_Analysis.png
│   ├── Marketing_Performance.png
│   ├── Operations_SLA.png
│   └── Customer_Returns.png
│
├── 📌 Data_Model/
│   ├── Star_Schema.png
│   └── Relationships_View.png
│
├── 📌 Dataset/
│   ├── FactSales_200k.csv
│   └── Dim_Tables_Info.md
│
├── 📌 DAX_Measures/
│   └── Key_DAX_Measures.md
│
├── 📌 PowerBI_File/
│   └── Ecommerce_Analytics.pbix
│
└── README.md

