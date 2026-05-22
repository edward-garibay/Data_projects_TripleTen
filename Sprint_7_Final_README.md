# Zomato Customer Analytics Dashboard

This was the seventh and final project that I worked on in the TripleTen Business Intelligence Analytics Program.  
It was a capstone project designed to showcase the full range of skills developed throughout the program using Power BI.  
The purpose was to analyze Zomato's customer base using two segmentation frameworks — RFM analysis and demographic segmentation — to identify the most valuable customers, at-risk segments, and data-driven strategies for improving retention and loyalty.

## Table of Contents for Repository Artifacts
| File Number | Title | Description |
| :---------: | ----- | ----------- |
| 1 | [README.md](README.md) | This current page with all relevant information about the project, just past the Table of Contents. |
| 2 | [Zomato.TB.pbix](Zomato.TB.pbix) | The Power BI file containing both dashboards and all visualizations. |
| 3 | [Zomato Customer Analytics Dashboard 2.pdf](Zomato%20Customer%20Analytics%20Dashboard%202.pdf) | Exported dashboard views for easy sharing and review. |
| 4 | [Zomato Customer Analytics Dashboard.pptx](Zomato%20Customer%20Analytics%20Dashboard.pptx) | Full presentation report with findings, recommendations, and next steps. |
| 5 | [Zomato data (2)](Zomato%20data%20(2)) | Source dataset containing all 5 Zomato data tables: food.csv, menu.csv, orders.csv, restaurant.csv, and users.csv. |

---

## Table of Contents for README
| Section Title | Description |
| ------------- | ----------- |
| [Description](#description) | Describes the final product's purpose, software, format, and included visuals. |
| [Process](#process) | A general outline of how this project formed from start to finish. |
| [Data](#data) | Describes the source of data, including files, tables, and fields. |
| [Assumptions](#assumptions) | Describes assumptions to include those given by TripleTen and assumptions made based on the data and task. |
| [Findings](#findings) | Insights learned from the data analysis. |
| [Recommendations](#recommendations) | Recommended direction for the stakeholders based on the final analysis. |

### Description:
- Two-dashboard Power BI report: a Demographic Segmentation Dashboard and an RFM Customer Segmentation Dashboard
- Includes KPI cards, trend lines, treemaps, and demographic breakdowns with full drill-down capability

### Process:
1) Selected the Customer Analysis Segmentation track from the three available capstone options.
2) Reviewed all 5 data tables (food, menu, orders, restaurant, users) and joined them as needed for customer-level analysis.
3) Built the Demographic Segmentation Dashboard analyzing customer profiles across age, gender, marital status, family size, education, income, and occupation — combined with business metrics.
4) Scored each customer on Recency, Frequency, and Monetary dimensions to calculate RFM scores.
5) Classified customers into 9 behavioral segments (Champions, At Risk, Hibernating, etc.) using RFM scores.
6) Built the RFM Dashboard with a treemap of all segments and drill-down metrics by RFM category.
7) Compiled findings and recommendations into a presentation-style report and PDF export.

### Data
The data was provided by TripleTen as 5 Zomato internal data tables:
- `'food'`: food item details
- `'menu'`: restaurant menu data
- `'orders'`: transaction and order records
- `'restaurant'`: restaurant information
- `'users'`: customer demographic and account data (age, gender, marital status, family size, education, income, occupation)

### Assumptions:
- RFM scoring is an appropriate framework for segmenting Zomato's customer base given the available transaction data.
- Demographic data in the `users` table is accurate and representative of the customer base.
- Monthly purchase frequency is a reliable proxy for customer engagement and loyalty trends.

### Findings:
**Demographics:**
1. The majority of users are aged 21–35; ages 19–25 generate the highest revenue.
2. Gender split: 58% male / 42% female.
3. 69% of users are single; average family size is 3.1 members.
4. Most users hold graduate or postgraduate degrees.
5. 32% report no income (likely students or early-career professionals) yet show high engagement and purchase volume.
6. Seasonal purchase spikes occur in August and December, likely tied to back-to-school and holiday shopping.

**RFM Segmentation:**
1. Hibernating customers make up 29% of the base — the largest segment — representing customers who haven't purchased recently.
2. Promising customers are 18% — high potential but not yet loyal.
3. Potential Loyalists are 12% — engaged customers close to moving into a loyalty tier.
4. Champions make up only 2% — the most valuable segment is significantly underdeveloped.
5. 20% of customers are At Risk or "Can't Lose Them" — requiring immediate re-engagement.
6. Ages 19–25 make up the majority of the Champions segment, suggesting strong ROI from targeting early-career customers.

### Recommendations:
1. Re-activate Hibernating and Promising segments with targeted promotional campaigns and personalized offers to push them toward loyalty tiers.
2. Launch re-engagement campaigns for At Risk users aged 22–26 using personalized discounts or limited-time offers tied to past purchase behavior.
3. Develop budget-friendly bundle deals for No Income and student users to drive upsell without alienating price-sensitive customers.
4. Close the gender gap by designing targeted incentives for female users to boost loyalty conversion and grow the 42% female segment.
5. Leverage seasonality — capitalize on August and December spikes with planned campaigns and introduce summer engagement strategies to offset the mid-year frequency dip.
6. Use in-app notifications to celebrate customer milestones (e.g., order anniversaries, loyalty tier upgrades) and encourage repeat orders.
