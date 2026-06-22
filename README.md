# E-Commerce Funnel Analytics

End-to-end funnel analysis on a real-world e-commerce dataset of **42.4 million events** spanning October 2019. Built to answer: *how do individual browsing sessions convert across the view → cart → purchase funnel?*

---

## Dashboard Preview
<img width="903" height="508" alt="Screenshot 2026-06-22 at 1 10 19 PM" src="https://github.com/user-attachments/assets/a512111c-74c6-4658-b326-711449922200" />


---


## Dataset
- **Source:** [Kaggle - eCommerce behavior data from multi category store](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store/data)
- **Size:** 42.4M rows, 9 columns
- **Period:** October 2019
- **Columns:** event_time, event_type, product_id, category_id, category_code, brand, price, user_id, user_session

---

## Tools & Technologies
- **Python** (Pandas, NumPy, Matplotlib, Plotly, Seaborn)
- **Jupyter Notebook**
- **Power BI Desktop**

---
## Key Findings

### 1. Funnel Anomaly — Direct Checkout Behavior
Purchase sessions (629K) exceeded cart sessions (573K). Investigation identified **337,699 sessions with a purchase event but no cart interaction**, indicating widespread use of direct "Buy Now" flows bypassing the cart stage. This is a structural platform behavior, not a data quality issue.

### 2. Massive Drop-off at View → Cart Stage
**93.8% of sessions** that viewed a product never added it to cart — the largest leakage point in the customer journey and the highest revenue opportunity.

### 3. Peak Conversion Hours: 4AM–9AM
Conversion rate peaked at **7.5–8%** during early morning hours, compared to 3.4% at midnight. Early morning shoppers exhibit significantly higher purchase intent.

### 4. Top Converting Category: Electronics Smartphones
`electronics.smartphone` achieved a **9.2% conversion rate** across 3.09M sessions — the highest volume and highest intent category simultaneously.

### 5. Brand Performance
Samsung (8.39%) and Apple (8.15%) led brand-level conversion among high-traffic brands, outperforming all competitors with significant session volume.

### 6. Day of Week Effect: Minimal
Conversion rate ranged only 6.44%–6.95% across all days of the week, suggesting promotional strategy should focus on **time-of-day targeting** rather than day-of-week.

---

## Dashboard Preview
<img width="903" height="508" alt="Screenshot 2026-06-22 at 1 10 19 PM" src="https://github.com/user-attachments/assets/c035c40c-aa08-4531-901b-f82e4d0a2dfb" />


---

## Analysis Sections
- Data cleaning & preprocessing (42.4M → deduplication → feature engineering)
- Session-level funnel aggregation
- User-level funnel aggregation
- Funnel anomaly investigation
- Brand-level conversion analysis
- Category-level conversion analysis
- Time-based analysis (hourly, daily, day-of-week)
- KPI summary & executive insights

---

## Business Recommendations
1. Audit and reduce view-to-cart drop-off — 93.8% leakage is the primary revenue opportunity
2. Deploy targeted campaigns in the 4AM–9AM window when purchase intent peaks
3. Prioritize `electronics.smartphone` and appliances categories for ad spend and inventory
4. Validate cart tracking infrastructure — 337K untracked cart events may be distorting funnel metrics


## Author

**Aryan Soni**

Data Analyst | Python | SQL | Tableau | PowerBI | Excel
