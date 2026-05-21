# From Reps to Results: A Deep Dive into the Top 50 Exercises

This was a collaborative project completed with teammates outside of the TripleTen Business Intelligence Analytics curriculum.  
It was a self-directed group project where Team TripleSet selected a fitness exercise dataset from a provided list and conducted an independent analysis.  
The purpose was to explore the effectiveness of the top 50 exercises through a data-driven lens and deliver actionable beginner workout plans backed entirely by data.

## Table of Contents for Repository Artifacts
| File Number | Title | Description |
| :---------: | ----- | ----------- |
| 1 | README.md | This current page with all relevant information about the project, just past the Table of Contents. |
| 2 | Project_Book_Version_7.twbx | The Tableau packaged workbook containing all dashboards and visualizations. |
| 3 | Top 50 Excerice for your body.csv | The source dataset — 50 exercises with sets, reps, calories burned, muscle groups, equipment, and difficulty level. |

---

## Table of Contents for README
| Section Title | Description |
| ------------- | ----------- |
| [Description](#description) | Describes the final product's purpose, software, format, and included visuals. |
| [Process](#process) | A general outline of how this project formed from start to finish. |
| [Data](#data) | Describes the source of data, including files, tables, and fields. |
| [Assumptions](#assumptions) | Describes assumptions made based on the data and research questions. |
| [Findings](#findings) | Insights learned from the data analysis. |
| [Recommendations](#recommendations) | Recommended direction for beginners based on the final analysis. |

### Description:
- Multi-view Tableau dashboard analyzing the top 50 exercises by muscle group, difficulty level, equipment use, and calorie burn
- Includes 6 visualizations and two structured beginner workout plans (with and without equipment)  
**Tableau Public** Share Link can be found [HERE](https://public.tableau.com/shared/FDPHTKKJ2?:display_count=n&:origin=viz_share_link)

### Process:
1) Selected the fitness exercise dataset from the list of provided options.
2) Explored the dataset to identify key dimensions: muscle group, difficulty level, equipment type, calorie burn, sets, and reps.
3) Defined research questions as a team and divided analysis across each dimension.
4) Built visualizations in Tableau covering muscle group frequency, calorie burn by difficulty, equipment vs. calorie comparisons, and beginner workout plans.
5) Created two structured beginner workout plans — one with no equipment and one with equipment — using filtered beginner-tier exercises from the dataset.
6) Compiled all views into a final Tableau summary dashboard.

### Data
The data was selected by the team from a list of provided datasets:
- `'Top 50 Excerice for your body.csv'`: each row represents one exercise
    - `'Name of Exercise'`: exercise name
    - `'Sets'`: recommended number of sets
    - `'Reps'`: recommended number of repetitions
    - `'Benefit'`: primary benefit of the exercise
    - `'Burns Calories (per 30 min)'`: estimated calorie burn per 30-minute session
    - `'Target Muscle Group'`: primary and secondary muscle groups targeted
    - `'Equipment Needed'`: equipment required (if any)
    - `'Difficulty Level'`: Beginner, Intermediate, or Advanced

### Assumptions:
- Calorie burn estimates (per 30 min) from the dataset are accurate and comparable across exercises.
- Review count of unique users (not sessions) at each funnel stage is the correct method for measuring conversion.
- No-equipment and equipment-based plans are compared fairly given the difference in available exercises at the beginner level in the dataset.
- Difficulty level classifications in the dataset accurately represent the physical demand of each exercise.

### Findings:
1. Glutes, Core, and Shoulders are the most frequently targeted muscle groups across the top 50 exercises.
2. There is a clear positive correlation between difficulty level and calories burned per 30 minutes:
    - Beginner: ~189 calories
    - Intermediate: ~224 calories
    - Advanced: ~279 calories
3. An inverse relationship exists between the number of muscle groups targeted and calories burned in beginner exercises — more isolated movements burn more calories per session at this level:
    - 1 muscle group: ~223 calories
    - 2 muscle groups: ~200 calories
    - 3 muscle groups: ~181 calories
4. Beginner no-equipment workout plan: 1,673 total calories burned / 351 total reps.
5. Beginner equipment-based workout plan: 600 total calories burned / 180 total reps.
6. No-equipment workouts result in a 1,073-calorie advantage over equipment-based plans at the beginner level, primarily due to higher available rep volume.

### Recommendations:
1. Beginners should prioritize Glutes, Core, and Shoulders in their programs — these are the most commonly trained and calorie-efficient muscle groups.
2. Effective, high-calorie-burning routines do not require expensive equipment — structured no-equipment workouts can outperform equipment-based plans in total calorie output.
3. As difficulty increases, so does calorie burn — beginners should progressively challenge themselves over time to maximize results.
4. Structure and consistency matter more than equipment access; following a planned routine will yield better results than random workouts regardless of available tools.
