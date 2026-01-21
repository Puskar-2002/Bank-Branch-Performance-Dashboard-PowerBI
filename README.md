
# 🏦 Bank Branch Performance Dashboard | Power BI
Interactive Power BI dashboard analyzing bank branch performance using KPIs, regional analysis, customer growth, NPA %, and city-level insights.

## 📌 Project Overview
The **Bank Branch Performance Dashboard** is an interactive Power BI report designed to evaluate the overall performance of a bank across **regions, branches, cities, and time periods**.

This dashboard provides a **single, consolidated view** of key banking metrics such as deposits, loans, profitability, customer growth, and credit risk (NPA).  
It enables management and business users to quickly identify **performance trends, risk areas, and growth opportunities** using interactive visuals and slicers.

The project is built as a **real-world banking analytics use case** and is suitable for portfolio presentation and interview discussions.

---
## 📊 Dashboard View

[![Bank Branch Performance Dashboard](Dashboard%20Power%20Bi.png)](https://github.com/Puskar-2002/Bank-Branch-Performance-PowerBI/blob/main/Dashboard%20Power%20Bi.png)

## 🧠 Business Problem
Banks operate through multiple branches spread across regions and cities. Tracking performance manually or through static reports makes it difficult to:

- Monitor overall profitability
- Identify high-risk regions with elevated NPAs
- Compare branch-level performance
- Track customer growth trends over time
- Take timely, data-driven decisions

This dashboard addresses these challenges by transforming raw banking data into **actionable visual insights**.

---

## 🎯 Project Objectives
- Provide an **executive-level performance summary**
- Monitor **key financial KPIs**
- Analyze **regional, branch, and city-level performance**
- Track **customer growth and attrition**
- Identify **credit risk using NPA %**
- Enable **interactive self-service analysis**

---

## 📊 Key Performance Indicators (KPIs)
The dashboard highlights six core KPIs at the top for quick decision-making:

- **Total Branches (10)**  
  Indicates the operational footprint of the bank.

- **Total Deposits (2bn)**  
  Reflects customer trust and liquidity strength.

- **Total Loans (1bn)**  
  Shows the bank’s total credit exposure.

- **Net Profit (13.17M)**  
  Represents overall profitability after expenses.

- **Customer Growth % (2.25%)**  
  Indicates a positive net increase in customers.

- **NPA %**  
  Measures credit risk relative to total loans.

These KPIs collectively provide a balanced view of **growth, profitability, and risk**.

---

## 📈 Dashboard Analysis & Insights

### 🔹 1. Regional Risk Analysis – *NPA % by Region*
- The **East region** shows the highest NPA %, indicating higher credit risk.
- Other regions (North, South, West) maintain relatively stable NPA levels.

**Insight:**  
The East region requires closer monitoring and stronger risk-control measures.

---
## 📂 Files in This Repository

| File Name | Description |
|---------|-------------|
| `Bank_Branch_Performance.pbix` | Main Power BI dashboard file |
| `Bank_Branch_Performance_Dataset.xlsx` | Dataset used for analysis |
| `Dashboard Power Bi.png` | Screenshot of the Power BI dashboard |
| `Measures_DAX.txt` | DAX measures used in the dashboard |
| `README.md` | Complete project documentation |


### 🔹 2. Revenue Contribution – *Total Revenue by Region*
- The **South region** contributes the highest share of total revenue.
- North and West follow closely, while East contributes the least.

**Insight:**  
The South region is the strongest revenue driver and presents opportunities for further expansion.

---

### 🔹 3. Geographic Performance – *Net Profit & NPA % by City*
- Bubble size represents **Net Profit**
- Tooltips display **NPA %**

Cities such as **Mumbai, Hyderabad, and Bengaluru** show strong profitability, while some cities show moderate profit with higher risk.

**Insight:**  
The map helps identify **high-profit but high-risk cities**, supporting balanced growth decisions.

---

### 🔹 4. Branch Performance – *Net Profit by Branch*
- Branches like **Banjara Hills** and **Anna Nagar** are top performers.
- Lower-ranked branches may require operational review.

**Insight:**  
Top branches can be used as benchmarks, while underperforming branches can be targeted for improvement.

---

### 🔹 5. Time-Based Trends – *Total Deposits by Month*
- Deposits peak in earlier months and gradually decline toward later months.
- A noticeable drop is observed toward the end of the period.

**Insight:**  
This trend may indicate seasonal effects, customer behavior changes, or the need for deposit mobilization strategies.

---

### 🔹 6. Interactive Filtering (Slicers)
The dashboard includes slicers for:
- **Region**
- **Month**
- **Branch Name**

These slicers dynamically update all visuals, enabling users to:
- Compare regions
- Analyze individual branches
- Focus on specific time periods

---

## 🧮 Data Model & Calculations
- The dashboard follows a **fact-dimension data model**
- All KPIs and metrics are created using **DAX measures**
- Measures are designed to be:
  - Accurate
  - Filter-aware
  - Reusable
  - Performance-optimized

### Example DAX Logic
```DAX
Net Profit =
SUM ( Fact_BranchPerformance[Revenue] )
- SUM ( Fact_BranchPerformance[Expense] )
DAX
Copy code
Customer Growth % =
DIVIDE (
    SUM ( Fact_BranchPerformance[New_Customers] )
    - SUM ( Fact_BranchPerformance[Closed_Customers] ),
    SUM ( Fact_BranchPerformance[Closed_Customers] ),
    0
)
🛠 Tools & Technologies
Power BI Desktop – Data modeling and visualization

DAX (Data Analysis Expressions) – Business logic

Microsoft Excel – Data source

Bing Maps – Geographic analysis

🖼️ Dashboard Preview

🚀 How to Use the Dashboard
Open the report in Power BI Desktop

Refresh the dataset if required

Use slicers to filter data by region, month, or branch

Hover over visuals and map bubbles to view detailed tooltips

📈 Business Value
Improves visibility into branch and regional performance

Helps identify risk-prone areas using NPA %

Supports strategic planning and operational improvements

Enables data-driven decision-making for banking leadership

👤 Author:

Puskar Sarkar
Aspiring Data Analyst | Excel | SQL | Power BI | Python
🔗 LinkedIn: https://www.linkedin.com/in/puskarsarkar02/
