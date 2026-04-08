# POS-System-Product-Analysis


##🧩 Background & Overview
A food delivery platform observed strong user engagement at the top of the funnel, with most users successfully reaching the menu.

However, a significant portion of users failed to convert from menu views into completed orders.

This project analyzes user behavior across the funnel to identify key drop-off points and quantify the impact of improving menu-to-order conversion.

Key Focus Areas:
Funnel conversion performance (Session → Menu → Order)
Conversion trends over time
Performance by region and restaurant size tier
Identification of top and underperforming restaurants
Modeled impact of improving conversion rates

##🗂️ Data Structure
The analysis is based on three core datasets:

funnel_weekly → Weekly funnel metrics (sessions, menu visits, orders)
restaurant_summary → Restaurant-level performance metrics
weekly_by_segment → Segmented performance (region, size tier)
Key Metrics:
Sessions
Orders
Menu-to-Order Conversion Rate (CVR)
Total Conversion Rate
The datasets were joined and aggregated to analyze performance across time, geography, and business segments.

##⚡ Executive Summary
The primary bottleneck in the funnel occurs after users reach the menu.

While upstream engagement remains strong, conversion from menu to order averages ~21.94%, representing the largest opportunity for growth.

Key findings:

Conversion rates are consistent across regions and size tiers, indicating systemic friction
Top-performing restaurants significantly outperform the average, suggesting optimization opportunities
A modeled +3 percentage point increase in CVR results in:
→ +13.64% relative lift
→ Significant increase in total orders at scale

This highlights post-menu optimization as the highest-leverage growth opportunity.

##📈 Conversion Trends
Menu-to-order conversion remained relatively stable over time (~21–22%) with minor fluctuations.

This suggests:

No major seasonality impact
Persistent structural inefficiencies in the ordering experience

##🌍 Segment Performance
Conversion rates across regions and size tiers showed minimal variation.

Implication:

The issue is not isolated to specific markets or business segments
Indicates platform-wide UX or product friction

##🏆 Restaurant Performance
Top-performing restaurants achieved CVRs above 34%, significantly outperforming the average (~22%).

Underperforming restaurants showed CVRs as low as ~9–12%.

Implication:

Best performers provide a benchmark for optimization
Opportunity to standardize high-performing behaviors across the platform


##💡 Recommendations
Based on the analysis, the primary focus should be improving post-menu conversion.

Suggested Actions:
Improve menu UX (clear pricing, layout, item visibility)
Reduce checkout friction (fewer steps, faster load times)
Introduce personalization (recommended items, bundles)
Analyze top-performing restaurants to identify best practices
These changes target the highest-leverage point in the funnel.

##🚀 Modeled Impact
Scenario: +3 percentage point increase in Menu-to-Order CVR

Current CVR: 21.94%
Projected CVR: 24.99%
Relative Lift: +13.64%
Business Impact:
At scale:

1,000,000 sessions → +30,000 additional orders
This demonstrates that small improvements in conversion can drive significant revenue growth.

##📊 Dashboard
The Tableau dashboard provides an interactive view of:

Conversion trends over time
Performance by region and size tier
Top and underperforming restaurants
Modeled impact of conversion improvements
🔗[https://public.tableau.com/views/PointofSaleProductFunnelAnalysis/FinalDashboardPOSFunnelAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link]

##🛠️ Technical Details
SQL (Databricks) for data transformation and aggregation
Tableau for visualization and dashboard design
Additional technical work:

Data cleaning and joins across multiple datasets
Aggregation of weekly and segment-level metrics
(See SQL queries in repository files)

##⚠️ Assumptions & Caveats
- Assumes consistent tracking of sessions and orders across time
- Does not account for external factors (promotions, pricing changes)
- Modeled impact assumes linear conversion improvement
- These factors may influence real-world results.

