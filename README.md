# AI-POWERED-BUSINESS-INTELLIGENCE-
# CODTECH-Task3

Name: ATLA UDAY KIRAN
Company: CODTECH IT SOLUTIONS
ID: CITS5172
Domain: DATA ANALYTICS
Duration: 18th JUNE 2026 to 16th JULY 2026
Mentor: NEELA SANTHOSH KUMAR

## 🤖 Project Overview: AI-Powered Business Intelligence

As part of my role at CODTECH IT SOLUTIONS, I built an AI-powered business
intelligence system on a synthetic multi-department business dataset. This
project combines traditional BI analysis (revenue, cost, profit trends) with
AI techniques — clustering, forecasting, and anomaly detection — to surface
deeper insights automatically.

### Objective

To apply AI/ML techniques on top of business data to automate insight
generation — including customer segmentation, revenue forecasting, and
detection of unusual transactions — going beyond standard dashboards.

### Steps Taken

**1. Data Generation and Loading:**
- Generated a synthetic dataset of 2,000 business records spanning 2023–2024.
- Features include Department, Region, Product, Revenue, Cost, Profit, Units Sold, Marketing Spend, and Customer Satisfaction.

**2. Exploratory BI Analysis:**
- Plotted monthly Revenue, Cost, and Profit trends on a single chart.
- Compared total revenue across Departments.
- Calculated and visualized Profit Margin % per Product.
- Built a Region × Department revenue heatmap.

**3. AI — Customer Segmentation (K-Means Clustering):**
- Applied K-Means (k=3) on Revenue, Units Sold, Marketing Spend, and Customer Satisfaction.
- Evaluated segment quality using the Silhouette Score.
- Visualized clusters on a Revenue vs Customer Satisfaction scatter plot.

**4. AI — Revenue Forecasting (Linear Regression):**
- Aggregated monthly revenue and fitted a Linear Regression trend model.
- Extended the forecast 6 months beyond the available data.
- Plotted actual revenue, trend line, and forecast together.

**5. AI — Anomaly Detection (Isolation Forest):**
- Trained an Isolation Forest model on Revenue, Profit, and Marketing Spend.
- Flagged the top 5% of records as anomalies.
- Visualized normal vs anomalous data points on a Revenue vs Profit scatter plot.

### Key Insights

- **Sales** department generates the highest total revenue across all regions.
- **Product C** achieves the highest profit margin despite lower absolute revenue.
- AI clustering identified 3 distinct business performance segments — high-value, mid-tier, and low-engagement.
- Revenue shows a steady upward trend; the 6-month forecast projects continued growth.
- **100 anomalous transactions** were flagged by Isolation Forest, indicating potential billing errors or unusual market events worth investigating.
- The **South** region consistently outperforms other regions across all departments.

### Conclusion

This project demonstrated how AI techniques can augment traditional business
intelligence. Rather than just reporting what happened, the AI models
explain patterns (clustering), predict what comes next (forecasting), and
flag what looks wrong (anomaly detection) — making BI proactive rather than
reactive.

---

## Output Graphs

### 1. Monthly Revenue, Cost & Profit Trend
<img width="1320" height="550" alt="01_revenue_cost_profit_trend" src="https://github.com/user-attachments/assets/46f59674-4684-42a2-ba93-a3445e665c7a" />
### 2. Total Revenue by Department
<img width="990" height="550" alt="02_revenue_by_department" src="https://github.com/user-attachments/assets/95453150-47d5-4898-b50c-275dd7435d6d" />

### 3. Profit Margin % by Product
<img width="990" height="550" alt="03_profit_margin_by_product" src="https://github.com/user-attachments/assets/811b21f6-6195-4756-b60c-57f86932094d" />

### 4. AI Customer Segmentation — K-Means Clustering
<img width="880" height="660" alt="04_customer_segmentation" src="https://github.com/user-attachments/assets/b82a21e7-fbcf-4fe6-8aa6-a0572cba9f09" />

### 5. AI Revenue Forecasting — Linear Regression
<img width="1320" height="550" alt="05_revenue_forecast" src="https://github.com/user-attachments/assets/b1d28a0d-d7ff-4397-a7a3-8a2c13d097fc" />

### 6. AI Anomaly Detection — Isolation Forest
<img width="1100" height="660" alt="06_anomaly_detection" src="https://github.com/user-attachments/assets/2de6bc53-6145-4391-ae9e-a461263242ad" />

### 7. Revenue Heatmap: Region vs Department
<img width="1100" height="550" alt="07_region_department_heatmap" src="https://github.com/user-attachments/assets/f802aa47-e97a-4653-9838-2bfa8b64ab05" />


## How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
python generate_data.py
python ai_business_intelligence.py
```

## Files in this Repository

| File | Description |
|---|---|
| `AI_Business_Intelligence.ipynb` | Full notebook with code and analysis |
| `ai_business_intelligence.py` | Main AI analysis and visualization script |
| `data/business_data.csv` | Generated dataset (2,000 rows) |
| `output/` | All generated chart images and summary stats |

