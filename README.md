# Phase-2-Project_Group-8-

# Film Production Analysis

Welcome to the **Film Production Analysis** project! This project, developed for the Moringa School Phase 2 Data Science curriculum, provides strategic business insights for a new movie studio. By analyzing historical data from 2010–2018, we identify the drivers of critical acclaim and commercial success to help stakeholders make data-driven decisions.

## Table of Contents

- [Project Overview](https://www.google.com/search?q=%23project-description)
- [Datasets Used](https://www.google.com/search?q=%23datasets-used)
- [Exploratory Data Analysis (EDA)](https://www.google.com/search?q=%23exploratory-data-analysis-eda)
- [Visualizations](https://www.google.com/search?q=%23visualizations)
- [Insights](https://www.google.com/search?q=%23insights)
- [Recommendations](https://www.google.com/search?q=%23recommendations)
- [Team](https://www.google.com/search?q=%23team)

## Project Description

Our company is entering the film industry and needs to understand what makes a movie "successful." This project integrates data from IMDb, Rotten Tomatoes, The Numbers, TMDb, and Box Office Mojo to analyze the relationships between genres, production budgets, and audience ratings.

## Datasets Used

| File Name              | Source          |
| ---------------------- | --------------- |
| `bom.movie_gross.csv`  | Box Office Mojo |
| `tn.movie_budgets.csv` | The Numbers     |
| `tmdb.movies.csv`      | TMDb            |
| `rt.movie_info.tsv`    | Rotten Tomatoes |
| `im.db`                | IMDb (SQLite)   |

## Exploratory Data Analysis (EDA)

**EDA Approach & process**

[Start]
↓
[Load Data]
├─ Load CSV & TSV files into DataFrames
└─ Convert SQLite database tables into DataFrames
↓
[Data Cleaning & Preparation]
├─ Check for missing values
├─ Handle inconsistencies
└─ Standardize column formats
↓
[Initial Data Exploration]
├─ Understand data structure
└─ Identify key columns
↓
[Identify Relationships]
├─ Detect common columns across datasets
└─ Select "title" as primary key
↓
[Data Integration]
├─ Join tables using INNER JOIN
└─ Merge datasets ON "title"
↓
[Save Merged Data]
├─ Export merged dataset as CSV
└─ Reload CSV into DataFrame
↓
[Exploratory Data Analysis]
├─ Perform descriptive statistics
└─ Generate visualizations & insights
↓
[End]

**Key findings from our analysis include:**

- **Genre and Quality Parity:** Statistical testing (ANOVA) confirms that high ratings are achievable across a variety of genres. There is no statistically significant difference in quality scores between "prestige" genres like Documentary or History and commercial ones like Animation ($p = 0.5967$), proving that quality is not limited to a single category.
- **Weak Link Between Ratings and Profit:** While a positive relationship exists, it is statistically weak. Higher-rated movies do not automatically guarantee high profits; ratings should be viewed as a secondary metric for brand reputation rather than a primary driver for financial investment.
- **Commercial Powerhouses:** Animation, Sci-Fi, and Adventure films generate the highest average worldwide profits. These genres demonstrate the strongest global appeal and represent the most reliable categories for sustainable revenue generation.
- **The Critical Importance of Timing:** The month of release is a major driver of profitability ($p < 0.05$). February, May, June, July, November, and December are peak months for profit, while "dump months" like January and September typically show much lower potential.
- **Domestic Success Predicts Global Reach:** We identified a strong positive correlation ($r \approx 0.73$) between domestic and worldwide gross. This makes domestic box-office performance a reliable leading indicator for a film's eventual global success.
- **Market Reach vs. Critical Acclaim:** Analysis suggests that a film's financial success is more heavily influenced by its genre selection and market reach than by its numeric critic rating alone.
- **Genre Consistency:** High audience ratings are not exclusive to any single genre; quality is achievable across diverse categories.
- **Budget Impact:** While blockbuster budgets drive massive worldwide gross, mid-range budgets often offer safer ROI margins.
- **Seasonal Trends:** Profitability fluctuates significantly by release month, with clear "peak seasons" for high-return films.

## Visualizations

We utilized `matplotlib` and `seaborn` to generate insights, focusing on the following areas:

- **Most Common Genres:** Identification of the most saturated vs. niche markets.
- **Ratings Distribution:** Visualizing how different genres compare in critical reception.
- **Financial Correlation:** Heatmaps showing the link between domestic performance and worldwide success.

## Insights

- **Statistical Parity in Quality:** Our ANOVA test (F=0.694, p=0.597) confirms there is **no statistically significant difference** in average ratings between top-performing genres like Documentary, History, and Animation.
- **Revenue vs. Rating Gap:** High critical acclaim (Prestige) does not always correlate with high profit. For example, Documentaries score high in quality but often struggle with ROI compared to Animation.
- **Domestic Predictor:** Domestic box office performance is a strong lead indicator for total worldwide revenue.

## Recommendations and Summary of Findings

## Ratings vs Genre

- Documentary, History, and Biology films receive the highest average ratings. However, an ANOVA test across genres shows no statistically significant difference in average ratings (F = 0.6941, p = 0.5967). This indicates that high ratings can occur in any genre, and ratings alone are not a reliable measure of a movie’s success.

## Ratings vs Profit

- The relationship between movie ratings and profit is positive but weak. Higher-rated movies tend to earn more, but ratings alone do not strongly determine profitability. This suggests that while good ratings help, they do not guarantee high financial success.

## Genre vs Worldwide Profit

- Animation, Sci-Fi, and Adventure films generate the highest average worldwide profits, demonstrating strong global appeal. This indicates that genre choice has a greater impact on revenue than ratings. Action and Adventure films, in particular, should be prioritized by the studio.

## Release Month vs Profit

- Statistical analysis shows that release month has a significant effect on movie profit (p < 0.05). Movies released in February, May, June, July, November, and December perform best, while releases in January, August, September, and October perform poorly. Timing is therefore a critical factor in maximizing profitability.

## Domestic vs Worldwide Performance

- There is a very strong positive correlation between domestic and worldwide gross (r ≈ 0.73, p ≈ 0). This means that movies that perform well domestically are very likely to perform well internationally. Domestic performance can be used as a leading indicator of global success.

### Final Conclusion & Recommendation

- Movie success is driven primarily by genre selection, release timing, and market reach, rather than ratings alone. While good ratings contribute positively, they should be treated as a secondary metric.

### Based on Analysis we Recommend

- Prioritize Genre for Profitability: Focus on producing Action, Adventure, Animation, and Sci-Fi movies, as these genres consistently generate the highest worldwide profits. Ratings are helpful but should not be the primary measure of expected success.

- Optimize Release Timing: Schedule movie releases in months with historically high profits: February, May, June, July, November, and December. Avoid releasing in January, August, September, and October, which show lower profit potential.

- Use Domestic Performance as a Predictor: Monitor domestic box office performance closely, as it is a strong indicator of worldwide success. Strong domestic earnings can help predict and maximize global revenue.

- Leverage Ratings Strategically: While high ratings do not guarantee profit, they can enhance a movie’s marketability. Use ratings as a secondary metric to guide marketing and audience targeting rather than as the primary decision factor for production or release strategy.

## Team

- **Geoffrey Kemboi** | [https://www.linkedin.com/in/geoffrey-kemboi-aiik-720345104/]
- **Peter Kiarie** | [https://www.linkedin.com/in/peter-kiarie-529232109/]
- **Natasha Wangare** | [www.linkedin.com/in/natasha-gitungo-b78212142/]
- **Samantha Jepkosgei** | [https://www.linkedin.com/in/jepkosgei-samantha-265364151/]
- **Elvis Okeyo** | [https://www.linkedin.com/in/okeyo-otieno-027257298/]
