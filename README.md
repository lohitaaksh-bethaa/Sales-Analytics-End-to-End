# End-to-End Sales Analytics & Profitability Dashboard

## Business Objective
The objective of this project is to analyze sales performance, profitability, customer behavior, and discount impact to support data-driven business decisions around pricing, regional strategy, and customer management.

This project simulates a real-world analytics workflow used by data teams to deliver reliable insights to management.

---

## Data Overview
- 50,000 transactional sales records
- Time period: 2022–2024
- Granularity: Order-level data
- Dimensions:
  - Region
  - Product
  - Customer
  - Date
- Key Metrics:
  - Revenue
  - Net Revenue
  - Profit
  - Discount %
  - Profit Margin

---

## Tech Stack
- **MySQL** – Data storage, indexing, and analytical SQL queries
- **Python (Pandas, Matplotlib)** – Data cleaning, feature engineering, EDA, automation
- **Excel** – Data validation, reconciliation, ad-hoc analysis
- **Power BI** – Data modeling, DAX measures, executive dashboards

---

## Project Architecture
Raw CSV
↓
MySQL (Data Storage & SQL Analysis)
↓
Python (Cleaning, Feature Engineering, EDA)
↓
Excel (Validation & Reconciliation)
↓
Power BI (Modeling, DAX, Dashboards)


---

## Key Insights & Business Recommendations

### Insight 1: Discounts Above 15% Reduce Profitability
**Observation:**  
Orders with discounts greater than 15% show a sharp decline in profit margins without proportional revenue growth.

**Evidence:**  
- SQL aggregation by discount percentage  
- Python groupby analysis on discount vs profit  
- Power BI Discount vs Profit dashboard  

**Business Impact:**  
Excessive discounting leads to margin erosion across regions.

**Recommendation:**  
Cap discounts at 10–15% and introduce targeted, customer-specific discounts.

---

### Insight 2: High Revenue Does Not Always Mean High Profit
**Observation:**  
Several products generate high revenue but contribute disproportionately low profit.

**Evidence:**  
- Product-level profit analysis in SQL  
- Scatter plot of Revenue vs Profit in Power BI  

**Business Impact:**  
Revenue-focused decisions can hide underlying inefficiencies.

**Recommendation:**  
Reprice or bundle low-margin products and define minimum margin thresholds.

---

### Insight 3: Revenue Concentration Risk Among Top Customers
**Observation:**  
Top 10 customers contribute a significant share of total revenue.

**Evidence:**  
- Customer revenue distribution in Power BI  
- Python aggregation by customer  

**Business Impact:**  
High dependency increases churn and negotiation risk.

**Recommendation:**  
Implement retention strategies for top customers and growth plans for mid-tier customers.

---

### Insight 4: Regional Margin Variations
**Observation:**  
Some regions generate strong revenue but lag in profitability due to higher discounts and cost structures.

**Evidence:**  
- Region-wise profit and margin analysis in SQL and Power BI  

**Business Impact:**  
Uneven profitability across regions affects overall business health.

**Recommendation:**  
Optimize pricing and discount strategies at a regional level.

---

### Insight 5: Seasonal Sales Patterns
**Observation:**  
Revenue and profit show clear seasonality with stronger performance in specific quarters.

**Evidence:**  
- Monthly and quarterly trend analysis in Power BI  

**Business Impact:**  
Inventory and marketing decisions can be better timed.

**Recommendation:**  
Increase inventory planning and promotional activity ahead of peak periods.

---

## Power BI Dashboard Overview
The Power BI report contains four pages:
1. **Executive Overview** – Revenue, profit, margin, and trends
2. **Product Performance** – Top/bottom products and margin analysis
3. **Customer Analysis** – Customer contribution and concentration risk
4. **Discount & Profitability** – Discount thresholds and margin impact

The data model follows a star schema with a dedicated Date table and optimized DAX measures.

---

## Data Validation & Quality Checks
- Excel pivot tables were used to reconcile totals across SQL, Python, and Power BI
- Data validation rules enforced for Region and Discount %
- Indexing applied in MySQL to optimize query performance

---

## Limitations & Future Enhancements
- Dataset does not include marketing spend or operational costs
- Customer segmentation can be enhanced using RFM analysis
- Future work could include forecasting, cohort analysis, and scenario modeling

---

## Repository Structure
Sales-Analytics-End-To-End/
│
├── BI File/  # Power BI dashboard (.pbix) and python exported .csv sorted source files.
├── Data Source File/ # Cleaned datasets
├── Excel/ # Validation and reconciliation files
├── Python Files/ # Jupyter notebook for analysis
├── SQL Files/ # SQL queries and scripts
└── README.md


---

## Author
**Lohitaaksh Bethaa**  
Data Analyst
