# Manhattan Airbnb Market Analysis

This was the second project that I worked on in the TripleTen Business Intelligence Analytics Program.  
It was an independent project designed to showcase what I have learned about advanced spreadsheet analysis using Google Sheets.  
The purpose was to analyze New York City Airbnb listing data and advise a client on the best neighborhoods and property sizes to invest in for vacation rentals in Manhattan.

## Table of Contents for Repository Artifacts
| File Number | Title | Description |
| :---------: | ----- | ----------- |
| 1 | README.md | This current page with all relevant information about the project, just past the Table of Contents. |
| 2 | [Full Analysis (Google Sheets)](https://docs.google.com/spreadsheets/d/1QHGYVy3Y4tYOP9_YG16oESJ6HqTrpEug4m3ta8fxzkw/edit?usp=sharing) | The spreadsheet containing all data cleaning, pivot tables, analysis, and revenue estimates. |

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
- Google Sheets analysis including data cleaning, pivot tables, and revenue modeling
- Structured to answer two core investment questions: best neighborhoods and best property sizes for Manhattan vacation rentals  
**Google Sheets** (Full Analysis) can be found [HERE](https://docs.google.com/spreadsheets/d/1QHGYVy3Y4tYOP9_YG16oESJ6HqTrpEug4m3ta8fxzkw/edit?usp=sharing)

### Process:
1) Cleaned the dataset — standardized neighborhood name capitalization, removed trailing spaces (`neighborhood_clean` column), and handled empty bedroom values representing studio apartments (`bedrooms_clean` column using `IF` function).
2) Documented all cleaning steps in a dedicated change log sheet.
3) Built pivot tables to rank the top 10 neighborhoods by review count over the last 12 months.
4) Analyzed the most popular property sizes overall and by neighborhood.
5) Created a `top_listing` flag (1/0) to filter listings matching the recommended neighborhood and size.
6) Calculated `revenue_earned` per night using `SUMIF()` across 30-day calendar data and projected annual revenue.

### Data
The data was provided by TripleTen as an NYC Airbnb dataset:
- `'listings'`: details all fields for each active rental listing
    - Key fields: `number_of_reviews_ltm`, `neighbourhood`, `bedrooms`, `adjusted_price`
- `'calendar'`: day-by-day availability and pricing for each listing
    - Key fields: `listing_id`, `available`, `adjusted_price`

### Assumptions:
- Review count over the last 12 months (`number_of_reviews_ltm`) is a reliable proxy for rental activity and demand.
- 30-day calendar revenue, multiplied by 12, provides a reasonable annual revenue estimate.
- Empty bedroom values in the dataset represent studio apartments (0 bedrooms).

### Findings:
1. The top 3 most attractive neighborhoods are Lower East Side, Hells Kitchen, and Harlem based on review volume.
2. Studios, 1-bedrooms, and 2-bedrooms dominate the top 10 neighborhoods by popularity.
3. 1-bedroom listings are the recommended property size for all top neighborhoods except Midtown, where studios are preferred.
4. Harlem specifically shows the strongest preference for 1-bedroom units.
5. The highest-earning listing (ID: 49946551) generated $29,940 over 30 days, projecting to approximately $359,280 annually.

### Recommendations:
1. Focus investment on 1-bedroom properties in Lower East Side, Hells Kitchen, and Harlem for the strongest combination of rental demand and revenue potential.
2. Consider studios in Midtown as a secondary opportunity given high tourist and business traveler traffic in that area.
3. Prioritize listings with a strong recent review history, as review volume is strongly correlated with rental demand.
