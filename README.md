#  Cohort & Customer Retention Analysis in E-commerce

##  Project Overview

This project tackles a critical issue in the e-commerce industry: **customer retention**.  
While many businesses are great at acquiring new customers, they often struggle to keep them. This leads to high marketing costs and low customer lifetime value (LTV).

Using real-world e-commerce transaction data, we performed a **cohort analysis** combined with **RFM segmentation** to deeply understand customer behavior, spending patterns, and loyalty.

---

## Business Goal

**E-Shop Pro**, our hypothetical e-commerce company, noticed declining retention rates and stagnating revenue growth — even though customer acquisition was increasing.

### The core business questions:
- When are we losing our customers?
- Which customers are most valuable?
- How can we improve long-term loyalty and revenue?

---

## Key Objectives

- Use **Cohort Analysis** to assess customer retention over time  
- Identify **top-performing and underperforming cohorts**
- Analyze **ARPU (Average Revenue Per User)** and **total revenue** per cohort
- Perform **RFM Segmentation** to classify customer behavior
- Provide actionable **insights and strategy** for marketing, retention, and growth

---

## 📊 Data Overview

| Column         | Description                                      |
|----------------|--------------------------------------------------|
| `InvoiceNo`    | Unique transaction ID                            |
| `StockCode`    | Product ID                                       |
| `Description`  | Product name                                     |
| `Quantity`     | Units purchased                                  |
| `InvoiceDate`  | Date and time of transaction                     |
| `UnitPrice`    | Price per unit                                   |
| `CustomerID`   | Unique ID for each customer                      |
| `Country`      | Country of the customer                          |

- Total records: **541,909**
- After cleaning: **4372 customers** retained for analysis

---

##  Analysis Performed

### 1. Cohort Analysis
- Grouped customers by their **first purchase month**
- Calculated **retention rate over 12+ months**
- Created a **heatmap** to visualize month-to-month retention

 **Insight**: Most cohorts drop by over 60% after Month 1 — early churn is the biggest risk.

---

###  2. Revenue & ARPU Analysis
- Tracked **total revenue per cohort**
- Calculated **ARPU (Avg Revenue Per User)** per cohort

 **Insight**: December 2010 cohort had both **high revenue and high ARPU** — a model cohort to replicate.  
 Recent cohorts showed **lower ARPU**, suggesting weaker acquisition quality.

---

###  3. RFM Segmentation
- Scored customers based on:
  - **Recency** (how recently they purchased)
  - **Frequency** (how often)
  - **Monetary** (how much they spent)
- Assigned scores (1–5) and labeled segments:
  -  Champions
  -  Loyal Customers
  -  At Risk
  -  Lost
  -  New Customers

**Insight**: ~10% of customers drive majority of revenue.  
 Most customers are one-time buyers with low engagement.

---

## Visuals & Deliverables

- ## 📊 Retention Heatmap
![Retention Heatmap](retention_heatmap.png) 

- ## Revenue & ARPU Bar Charts
  ![ARPU Chart](arpu_by_cohort.png)
  
  ![total revenue Chart](total_revenue_by_cohort.png)
  
- ## RFM Scatter Plot (Recency vs Frequency, bubble = Spend)
   ![RFM Scatter plot](rfm_scatter_plot.png)
  
- ## Segment Distribution Charts (Bar + Pie)
  
-  ![distribution pie chart](rfm_segment_distribution_pie.png)
  
- Export-ready PNG files

---

##  Key Business Recommendations

1. **Double down on what worked in December 2010**  
   → Campaigns, timing, offers, or onboarding that boosted long-term loyalty

2. **Introduce loyalty/reward programs**  
   → To convert one-time buyers into repeat customers

3. **Run reactivation campaigns** for at-risk and lost users  
   → Personalized emails, discounts, product reminders

4. **Identify & model high-ARPU customers**  
   → Use RFM profiles to target lookalikes in future acquisition

---

## Tech Stack

- **Python**
- **Pandas, NumPy** — data cleaning and analysis
- **Matplotlib, Seaborn** — visualization
- **Jupyter Notebook** — interactive development

---

## 📂 Project Files

| File Name                        | Description                       
|----------------------------------|-----------------------------------
| `cohort_retention_heatmap.png`  | Retention heatmap visualization   
| `total_revenue_by_cohort.png`   | Total revenue bar chart           
| `arpu_by_cohort.png`            | ARPU chart                       
| `rfm_scatter_plot.png`          | RFM scatter plot                    
| `rfm_segment_distribution_pie.png` | RFM segment share pie chart      

---

## OLUWASEYI Note

> This project was built as part of my personal growth in data analytics — a way to sharpen my cohort modeling and customer segmentation skills, while also staying close to solving real business problems.
> 
> Shoutout to everyone out there job-hunting, learning, or pivoting — keep going.  
> This one’s for the builders. 💪

---

## 📫 Let’s Connect

- [LinkedIn](#)


## 🚀 Project Status

✅ Cohort + RFM complete  
🔜 Next: Possible LTV prediction, churn modeling, or dashboard version (Power BI/Tableau)


