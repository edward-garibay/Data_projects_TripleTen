# E-Commerce Business Analytics: Conversion Funnel & Cohort Analysis

This was the third project that I worked on in the TripleTen Business Intelligence Analytics Program.  
It was an independent project designed to showcase what I have learned about business analytics using Google Sheets.  
The purpose was to turn raw e-commerce transaction logs into two key business metrics: a conversion funnel showing how users move from product views to purchases, and a cohort-based retention analysis tracking customer behavior month over month.

## Table of Contents for Repository Artifacts
| File Number | Title | Description |
| :---------: | ----- | ----------- |
| 1 | README.md | This current page with all relevant information about the project, just past the Table of Contents. |
| 2 | [Full Analysis (Google Sheets)](https://docs.google.com/spreadsheets/d/17NkhTIqAJLeRuq2rzPVGVNWVSBzOAK2F2Q77yeK5ddk/edit?usp=sharing) | The spreadsheet containing all raw data, pivot tables, conversion funnel, cohort analysis, retention rates, and executive summary. |

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
- Google Sheets analysis including a 3-stage conversion funnel, cohort-based retention analysis, and executive summary
- Organized across multiple sheets: Table of Contents → Executive Summary → Analytical Results → Calculation Sheets → Raw Data  
**Google Sheets** (Full Analysis) can be found [HERE](https://docs.google.com/spreadsheets/d/17NkhTIqAJLeRuq2rzPVGVNWVSBzOAK2F2Q77yeK5ddk/edit?usp=sharing)

### Process:
1) Built a 3-stage conversion funnel using a pivot table: Product Page View → Shopping Cart → Purchase.
2) Counted unique users at each funnel stage to avoid double-counting sessions; calculated total and step-to-step conversion rates.
3) Filtered raw activity logs to isolate purchase events only (`purchase_activity` sheet — 4,844 rows).
4) Created a `first_purchase` pivot table to identify each user's earliest purchase date.
5) Used `VLOOKUP()` to bring `first_purchase_date` into the purchase activity sheet for each user.
6) Used `TEXT()` to extract `event_month` and `first_purchase_month` in YYYY-MM format.
7) Used `DATEDIF()` to calculate `cohort_age` (0–4 months) for each purchase relative to a user's first purchase.
8) Built a `cohort_analysis` pivot table grouping users by first purchase month and a `retention_rates` sheet calculating month-over-month retention percentages.

### Data
The data was provided by TripleTen as a raw user activity log:
- `'raw_user_activity'`: each row represents a single user event on the e-commerce platform
    - `'user_id'`: unique customer identifier
    - `'event_type'`: page view, shopping cart, or purchase
    - `'category_code'`: product category
    - `'brand'`: product brand
    - `'price'`: product price at time of event
    - `'event_date'`: date the event occurred

### Assumptions:
- Review count of unique users (not sessions) at each funnel stage is the correct method for measuring conversion.
- A user's earliest purchase date is used to assign them to an acquisition cohort.
- Cohort age is calculated in full months using `DATEDIF()`, where month 0 = the first purchase month.

### Findings:
1. The 3-stage conversion funnel reveals drop-off rates at each stage of the buying journey from product page view to purchase.
2. Six acquisition cohorts were tracked across up to 4 months of post-purchase activity.
3. Cohort ages range from 0 to 4 months, capturing short-term repeat purchase behavior.
4. Retention rates vary by cohort, revealing which acquisition months produced the most loyal returning customers.

### Recommendations:
1. Investigate the largest drop-off stage in the conversion funnel and test targeted interventions (e.g., cart abandonment emails, simplified checkout) to improve step-to-step conversion.
2. Identify the highest-retention cohorts and analyze what differentiated those acquisition months — replicate those conditions in future campaigns.
3. For low-retention cohorts, design re-engagement campaigns (e.g., personalized discount codes, loyalty incentives) to recover lapsed customers before they churn entirely.
4. Monitor cohort behavior beyond 4 months to build a longer-term view of customer lifetime value by acquisition period.
