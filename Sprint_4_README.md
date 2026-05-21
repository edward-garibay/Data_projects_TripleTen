# Superstore Profitability vs. Returns

This was the fourth project that I worked on in the TripleTen Business Intelligence Analytics Program.  
It was an independent project designed to showcase what I have learned about Tableau Visualization.  
The purpose was to consult the company by reviewing the store's operations and identifying which areas of the business were driving losses versus profits.

## Table of Contents for Repository Artifacts
| File Number | Title | Description |
| :---------: | ----- | ----------- |
| 1 | DataSet - SuperStore.xls | The original data file provided by TripleTen that was used in the analysis of this project. |
| 2 | README.md | This current page with all relevant information about the project, just past the Table of Contents. |
| 3 | Sprint 4 Project.twbx | The Tableau packaged workbook containing all visualizations and dashboards. |

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
- 7-page Tableau Visualization
- Includes data analysis, charts, and an interactive dashboard.  
**Tableau Public** Share Link can be found [HERE](https://public.tableau.com/app/profile/edward.garibay/viz/Sprint4Project_17412121248390/Profitabiltyvs_Returns)

### Process:
1) Left Joined `'returns'` table to `'orders'` table.
2) Determined profit and loss centers by sub-category and region.
3) Analyzed product-level profitability to identify specific items generating losses.
4) Created a Calculated Field — `IF` formula for a Return Rate Measurement.
5) Examined the contribution of returns across various dimensions to overall profit.
6) Built a dashboard to visualize profitability vs. return rate by product.

### Data
The data was one Excel spreadsheet file provided by TripleTen:
- `'Superstore.xls'`: Each row corresponds to one product sold
    - `'orders'`: details all fields for each ordered item
    - `'returns'`: details all fields for each returned item

### Assumptions:
- Profits from sales are totaling in the negative.
- There is one or more causes for negative profits directly related to orders and returns.
- The operations department will need to make changes to avoid bankruptcy.
- The advertising department needs targeted recommendations based on profitable regions and seasons.

### Findings:
1. Sub-category profit centers are Copiers, Phones, and Accessories; loss centers are Tables, Bookcases, and Supplies.
2. Profit Centers by region are Office Supplies and Technology in the West; loss centers are Office Supplies and Furniture in the Central region.
3. Several individual products are causing negative profits, some with losses as high as $20K.
4. Advertising campaigns should target Indiana in October, Vermont in November, and Washington in March based on profitability patterns.
5. Returns are a significant problem, with many products having return rates as high as 100%.
6. Several customers have return rates as high as 100%.
7. When comparing average profit vs. return rate, certain individual products are not worth selling.

### Recommendations:
1. Continue to optimize sales and marketing efforts in profit centers (Copiers, Phones, Accessories) to maintain profitability.
2. Conduct a thorough analysis of loss centers (Tables, Bookcases, Supplies) — consider product adjustments, pricing strategies, or discontinuing consistently negative-profit items.
3. Investigate products with negative profits. If they consistently generate losses, consider removing them from inventory.
4. Target advertising campaigns by allocating budgets of 1/5 of a state's monthly profits during their most profitable seasons.
5. Investigate high return rates as a significant contributor to negative profits and take corrective action at the product level.
6. Analyze customer behavior to identify repeat returners and implement customer loyalty or support programs to address root causes.
