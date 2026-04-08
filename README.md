# 📊 POS System Product Funnel Analysis

## 🧩 Background & Overview

A food delivery platform observed strong user engagement at the top of the funnel, with most users successfully reaching the menu.

However, a significant portion of users failed to convert from **menu views → completed orders**.

This project analyzes user behavior across the funnel to:
- Identify key drop-off points  
- Quantify conversion inefficiencies  
- Model the impact of improving conversion rates  

### 🔍 Key Focus Areas
- Funnel performance (**Session → Menu → Order**)  
- Conversion trends over time  
- Performance by region & restaurant size tier  
- Identification of top vs. underperforming restaurants  
- Modeled impact of conversion improvements  

---

## 🗂️ Data Structure

The analysis is based on three core datasets:

| Dataset Name          | Description |
|----------------------|------------|
| `funnel_weekly`      | Weekly funnel metrics (sessions, menu visits, orders) |
| `restaurant_summary` | Restaurant-level performance metrics |
| `weekly_by_segment`  | Segmented performance (region, size tier) |

### 📌 Key Metrics
- Sessions  
- Orders  
- Menu-to-Order Conversion Rate (**CVR**)  
- Total Conversion Rate  

Datasets were joined and aggregated to analyze performance across:
- Time  
- Geography  
- Business segments  

---

## ⚡ Executive Summary

The primary bottleneck occurs **after users reach the menu**.

- Average Menu → Order CVR: **~21.94%**  
- This represents the **largest opportunity for growth**

### 🔑 Key Findings
- Conversion rates are consistent across regions and size tiers → indicates **systemic friction**  
- Top-performing restaurants significantly outperform the average → suggests **replicable best practices**  
- A **+3 percentage point increase in CVR** results in:
  - **+13.64% relative lift**  
  - Significant increase in total orders at scale  

👉 **Conclusion:** Post-menu optimization is the highest-leverage opportunity.

---

## 📈 Conversion Trends

- CVR remained stable (~21–22%) over time  
- Minimal fluctuation  

### 📌 Implications
- No major seasonality effects  
- Indicates **persistent structural inefficiencies** in the ordering experience  

---

## 🌍 Segment Performance

- Conversion rates show minimal variation across:
  - Regions  
  - Restaurant size tiers  

### 📌 Implications
- Issue is **platform-wide**, not localized  
- Likely caused by **UX / product friction**

---

## 🏆 Restaurant Performance

| Category            | CVR        |
|--------------------|-----------|
| Top Performers     | **> 34%** |
| Average            | **~22%**  |
| Underperformers    | **~9–12%**|

### 📌 Insights
- High performers provide a clear optimization benchmark  
- Opportunity to standardize winning behaviors across the platform  

---

## 💡 Recommendations

Focus on improving **post-menu conversion**.

### 🚀 Suggested Actions
- Improve menu UX  
  - Clear pricing  
  - Better layout  
  - Improved item visibility  
- Reduce checkout friction  
  - Fewer steps  
  - Faster load times  
- Introduce personalization  
  - Recommended items  
  - Bundles  
- Analyze top-performing restaurants  
  - Extract replicable best practices  

---

## 🚀 Modeled Impact

### Scenario: +3 percentage point increase in CVR

| Metric         | Value    |
|---------------|---------|
| Current CVR   | 21.94%  |
| Projected CVR | 24.99%  |
| Relative Lift | +13.64% |

### 📊 Business Impact

At scale:
- **1,000,000 sessions → +30,000 additional orders**

👉 Small improvements in conversion = **massive revenue impact**

---

## 📊 Dashboard

The Tableau dashboard provides an interactive view of:
- Conversion trends over time  
- Segment performance (region & size tier)  
- Restaurant-level performance  
- Modeled impact scenarios  

🔗 [View Dashboard](https://public.tableau.com/views/PointofSaleProductFunnelAnalysis/FinalDashboardPOSFunnelAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

## 🛠️ Technical Details

### Tools Used
- **ChatGPT** → Data generation inspired by Toast POS 10k Annual Report
- **SQL (Databricks)** → Data transformation & aggregation  
- **Tableau** → Visualization & dashboard design  

### Key Work
- Data cleaning across multiple datasets  
- Complex joins and aggregations  
- Weekly + segment-level performance modeling  

📂 See SQL queries in repository files.

---

## ⚠️ Assumptions & Caveats

- Assumes consistent tracking of sessions and orders  
- Does not account for external factors (e.g., promotions, pricing changes)  
- Modeled impact assumes linear conversion improvement  

👉 Real-world results may vary.
