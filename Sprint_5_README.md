# Superstore Returns Analysis

This was the fifth project that I worked on in the TripleTen Business Intelligence Analytics Program.  
It was an independent project designed to showcase what I have learned about Tableau Dashboards and Story Telling.  
The purpose was to prepare an analysis for the CEO of Superstore to help them understand what is causing customers to return their orders and how to reduce the volume of returned orders.

## Table of Contents for Repository Artifacts
| File Number | Title | Description |
| :---------: | ----- | ----------- |
| 1 | [Superstore.xls](Superstore.xls) | The original data file provided by TripleTen that was used in this project's analysis. |
| 2 | [README.md](README.md) | This current page with all relevant information about the project, just past the Table of Contents. |
| 3 | [Sprint 5 Project.twbx](Sprint%205%20Project.twbx) | The Tableau packaged workbook containing all visualizations, dashboard, and story presentation. |

---

## Table of Contents for README
| Section Title | Description |
| ------------- | ----------- |
| [Description](#description) | Describes the final product's purpose, software, format, and included visuals. |
| [Process](#process) | Describes the process, including the tools or techniques used. |
| [Data](#data) | Describes the data source, including files, tables, and fields. |
| [Assumptions](#assumptions) | Describes assumptions to include those given by TripleTen and assumptions made based on the data and task. |
| [Findings](#findings) | Insights learned from the data analysis. |
| [Recommendations](#recommendations) | Recommended direction for the stakeholders based on the final analysis. |

### Description:
- 9 Tableau Visualizations, 1 Dashboard, and a multi-page Story Presentation
- Includes data analysis, charts, a monitoring dashboard, and a Tableau story  
**Tableau Public** Share Link can be found [HERE](https://public.tableau.com/app/profile/edward.garibay/viz/Sprint5Project_17428429342910/ReturnRateByState)

### Process:
1) Left Joined `'returns'` table to `'orders'` table.
2) Created a Calculated Field — `IF` formula for a Return Rate Measurement.
3) Examined the in-depth contribution of returns across various dimensions using visualizations to determine what is causing returns.
4) Built a dashboard for monitoring returns across geography, product, and customer segments.
5) Created a Tableau story to present findings across 9 chapters.

### Data
The data was one Excel spreadsheet file provided by TripleTen:
- `'Superstore.xls'`: Each row corresponds to one product sold
    - `'orders'`: details all fields for each ordered item
    - `'returns'`: details all fields for each returned item

### Assumptions:
1) Profits from sales are totaling in the negative.
2) There is one or more causes for negative profits directly related to orders and returns.
3) The operations department will need to make changes to reduce return volume.

### Findings:
- Sales and returns are positively correlated — sub-categories with higher sales (Binders: 1,938 sales / 552 returns; Paper: 1,734 sales / 487 returns) also have the highest absolute return counts.
- Return rates are relatively consistent across product categories: Furniture 25.60%, Office Supplies 25.68%, Technology 27.33%.
- 60 customers have return rates above 47%, with the highest at 100%.
- Utah (56.84%) and California (45.17%) have the highest state-level return rates, yet both remain profitable.
- Texas is the most unprofitable state despite a moderate return rate of 13.43%.
- Fall season sees the highest return rates, with August (0.43) and December (0.34) peaking — likely tied to back-to-school and holiday shopping.
- September is the highest revenue and most profitable month despite elevated fall return rates.

### Recommendations:
1) Survey high-return customers (those above 50% return rate) to identify root causes and implement corrective measures.
2) Reach out to customers with a 100% return rate to determine the reasons behind their decisions; implement any needed changes to the website or shipping partners.
3) As triage, immediately stop selling problem products with consistently high return rates and negative profits.
4) Improve product listings with more accurate descriptions, sizing charts, detailed images, and customer reviews to reduce purchase uncertainty.
5) Apply targeted interventions in Texas to address profitability issues, which are independent of return rates.
6) Adjust promotional strategies for seasonal peaks — promote gift cards for the holidays and shift from discounts to value-added incentives like free shipping.
