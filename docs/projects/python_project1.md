# Project 1: Customer Segmentation Analysis using K-Means clustering

**Objective:**  
This project analyzes customer purchase behavior using **RFM analysis** and **K-Means clustering**, uncovering key customer groups and behavioral patterns.  
The insights are designed to support marketing and CRM teams in **personalized targeting, retention, and campaign optimization**.

---

## Data Overview

**Data Period:** April 1st – June 30th, 2025  
**Datasets Used:**
- `sales`: order-level data (sale_id, sale_date, customer_id, order_amount, country, channel)  
- `sales_item`: item-level data (product_id, price, quantity, customer_id, sale_id)  
- `customer`: demographic data (customer_id, age_range, signup_date, country)  

---

## Analytical Approach

1. **RFM Segmentation**  
   - Recency, Frequency, Monetary scoring to categorize customers:
     - 🏆 *Champions* — high frequency, high recency, high value  
     - 💎 *Loyal customers* — frequent and recent buyers  
     - ⚠️ *At-risk customers* — long inactive but historically high spenders  
     - 💔 *Lost customers* — inactive, low engagement  

2. **Behavioral Deep Dive**  
   - Purchase interval and time-of-day trends  
   - Channel reliance (e.g., website vs. app)  
   - Product category preference and average order value  
   - Demographic persona differences  
   - Lifecycle analysis: registration-to-first-purchase time  

3. **Clustering with K-Means**  
   - Behavioral feature normalization  
   - Elbow method for optimal k  
   - Cluster interpretation by product preference, spend, and recency  

---

## Key Insights

- **High-value customers**  (Champions) drive ~60% of total revenue; mostly aged 25–34, prefer direct web channel.  
- **At-risk customers**  show a declining trend in frequency; targeted reactivation campaigns can be designed around seasonal promotions.  
- **Loyal customers**  respond strongly to product category discounts, suggesting potential for personalized bundling.  
- **Lost customers**  tend to have short early engagement — onboarding optimization could extend lifecycle.  

---

## GitHub Repository  

🔗 [View the full project on GitHub →](https://github.com/Huistorical/Code/blob/main/rfm.ipynb)

Includes:
- Jupyter Notebook (`customer_segmentation.ipynb`)
- Data structure overview
- Python scripts and visualization code
- Tableau export instructions

---

## Tools & Stack  

| Category | Tools Used |
|-----------|-------------|
| Data Cleaning | pandas, numpy |
| Analysis | scikit-learn (KMeans), matplotlib, seaborn |
| Segmentation | RFM scoring, clustering |
| Visualization | Tableau, matplotlib |
| Documentation | MkDocs (Material theme) |

---

## Next Steps  

- Integrate real-time RFM updates into CRM dashboard  
- Automate customer churn alerts using scheduling tools  
- A/B test personalized marketing strategies per segment  

