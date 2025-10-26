
# 🛍️ E-Commerce User Behavior & Retention Analysis

** https://public.tableau.com/app/profile/abhishek.singh88/viz/Ecommerce_17453510821150/Dashboard1 **

This project analyzes customer behavior from an e-commerce store using techniques like A/B testing, segmentation, and cohort analysis. It aims to uncover insights to improve user retention, monetization, and business performance.

## 📁 1. Introduction

- Dataset: Online Retail data from a UK-based store (Dec 2010–Dec 2011)
- Objective: Understand customer value, improve revenue, and test strategies
- Tools Used: Python (Pandas, Matplotlib, Seaborn), StatsModels, Scipy
- Core Techniques: RFM Segmentation, A/B Testing, Multivariate Testing, Cohort Analysis

## 📊 2. Data Description

- ~500,000 transactions  
- Fields include: InvoiceDate, CustomerID, Quantity, UnitPrice, Country, Description
- Only UK customers with non-cancelled transactions were used  
- A new field "Revenue = Quantity × UnitPrice" was created

## 🎯 3. Business Impact

- Identify high-value users and segments
- Simulate pricing/discount strategies
- Analyze long-term behavior to improve retention
- Build actionable insights for marketing & product teams

## 🧩 4. Segmentation – RFM Analysis

- RFM = Recency, Frequency, Monetary
- Customers grouped into RFM scores (e.g., 444 = best)
- Key Findings:
  - 460 customers were in the top RFM 444 segment
  - Average revenue for 444s: £7,948
  - These customers are high repeat buyers and should be prioritized

## 🧪 5. A/B Testing – Discount Simulation

- Simulated 50/50 split: Test Group (10% discount) vs Control Group
- Metrics:
  - Conversion Rate
  - ARPU (Average Revenue per User)
- Result:
  - Control group outperformed test group
  - No statistically significant improvement in ARPU (p = 0.33)
  - Blanket discounting may not be effective

## 🧪 6. Multivariate Testing – Discount × Category

- Tested combinations of:
  - discount_flag (yes/no)
  - product category (Clothing, Home, Toys, Other)
- Key Insights:
  - Discount alone was not significant (p = 0.37)
  - No interaction between discount and category
  - Product category had some effect (p ≈ 0.05)
  - Better to focus on category-level strategies

## 📆 7. Cohort Analysis – Retention

- Grouped customers by first purchase month
- Tracked retention for next 12 months
- Insights:
  - December 2010 cohort had best long-term retention (e.g., 50% still active in Month 11)
  - Most cohorts drop to ~20–30% by Month 3
  - February to April 2011 cohorts show mid-retention improvements

## 💰 8. Cohort Analysis – Revenue

**Total Revenue by Cohort:**
- December 2010 generated the highest overall revenue across all months
- March and May cohorts showed spikes in later months

**Avg Revenue per User:**
- Normalized to remove cohort size bias
- August 2011 cohort peaked at £1,218 per user in Month 3
- May 2011, Month 7 had an outlier (£7,696 per user)
- Helps identify user quality, not just quantity

## ✅ 9. Summary

This project walks through the full customer analytics lifecycle using real-world e-commerce data. Each technique contributes to understanding how users behave, spend, and stay—helping businesses make better decisions.

- Exploratory Data Analysis (EDA):  
  Helped identify trends in daily revenue, best-selling products, and user geography—setting the foundation for deeper analysis.

- RFM Segmentation:  
  Categorized customers into Recency, Frequency, and Monetary groups. The top segment (RFM 444) showed extremely high lifetime value and strong engagement, revealing a clear target group for loyalty or premium programs.

- A/B Testing:  
  Simulated a discount campaign across two groups. Results showed no significant uplift in conversion or revenue, suggesting that flat discounts may not be effective across the entire user base.

- Multivariate Testing:  
  Tested discount performance across different product categories. Results showed no significant interaction between discount and category, but product type alone had some effect—highlighting the importance of category-specific strategies.

- Cohort Analysis (User Retention):  
  Tracked user return behavior by signup month. The December 2010 cohort retained users far longer than others—50% still active after 11 months—indicating a successful acquisition or seasonality effect.

- Cohort Analysis (Revenue-Based):  
  Analyzed both total revenue and average revenue per user. While larger cohorts like Dec 2010 generated high total revenue, normalized analysis showed August 2011 users had the highest average spend in Month 3, revealing hidden value in smaller segments.

## 💡 10. Business Recommendations

- Prioritize RFM 444 customers for loyalty and upsell offers
- Don’t rely on flat discounts—did not improve revenue
- Segment by product category before offering promos
- Improve onboarding for cohorts with early drop-off
- Use cohort analysis monthly to monitor retention strategies

** ChatGPT was used to summarize the whole project
