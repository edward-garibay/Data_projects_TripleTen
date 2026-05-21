# Shopify App Store Analysis

This was the sixth project that I worked on in the TripleTen Business Intelligence Analytics Program.  
It was an independent project designed to showcase what I have learned about data visualization and business analytics using Power BI.  
The purpose was to analyze the Shopify App Store ecosystem to understand what drives app ratings, review volume, and developer engagement across 7,341 apps.

## Table of Contents for Repository Artifacts
| File Number | Title | Description |
| :---------: | ----- | ----------- |
| 1 | README.md | This current page with all relevant information about the project, just past the Table of Contents. |
| 2 | Shopify App Store Analysis.pbix | The Power BI file containing all visualizations and dashboard pages. |

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
- Multi-page Power BI dashboard analyzing the Shopify App Store ecosystem
- Includes KPI cards, a line chart, scatter plot, and two bar charts examining app ratings, review volume, and developer behavior

### Process:
1) Connected to the Shopify App Store dataset in Power BI and reviewed all available fields.
2) Built KPI cards summarizing total app count and average helpful reviews.
3) Created a line chart to visualize review count trends over time by last modified date.
4) Built a scatter plot comparing average rating vs. reviews count to identify engagement patterns.
5) Created a bar chart comparing average ratings between apps where developers answered reviews and those that did not.
6) Built a bar chart ranking the top developers by total rating volume on the platform.

### Data
The data was provided by TripleTen as a Shopify App Store dataset:
- 7,341 apps represented across all categories
    - `'App ID'`: unique identifier for each app
    - `'Rating'`: average user rating
    - `'Reviews Count'`: total number of reviews received
    - `'Helpful Reviews'`: count of reviews marked as helpful
    - `'Developer Answered'`: whether the developer responded to reviews
    - `'Developer Name'`: name of the app developer
    - `'Last Modified Date'`: most recent update date for the app listing

### Assumptions:
- Review count and rating are the primary indicators of app success and user engagement.
- Helpful reviews are a meaningful proxy for review quality.
- Developer responsiveness (answering reviews) is a measurable signal of developer engagement.

### Findings:
1. 7,341 apps are available in the Shopify App Store.
2. The majority of apps maintain an average rating above 4.0 out of 5; fewer than 20 apps fall below this threshold.
3. Only 2 apps exceed 10,000 reviews, highlighting a significant concentration of engagement in a small number of listings.
4. Average helpful reviews across all apps is 5.48.
5. A spike in review volume was observed in early May, followed by stabilization — potentially tied to a platform promotion or algorithm change.
6. Apps where developers answered reviews show a different average rating pattern compared to those without developer responses.
7. Top developers by total rating volume: Hextom (~150K), Privy (~110K), Automize (~80K), followed by Shopify, CartKit, and Booster Apps.

### Recommendations:
1. Developers looking to grow on the platform should prioritize responding to reviews — developer responsiveness appears to influence user perception and ratings.
2. Invest in review generation strategies (e.g., in-app prompts, follow-up emails) to increase review volume, as very few apps break the 10,000-review threshold.
3. Study the top developers (Hextom, Privy, Automize) for best practices in product quality, marketing, and customer engagement.
4. Investigate the May review volume spike to determine if platform-level promotions or events drive meaningful engagement — and time launches accordingly.
