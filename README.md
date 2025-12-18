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

- **Genre and Quality Parity:** Statistical testing (ANOVA) confirms that high ratings are achievable across a variety of genres. There is no statistically significant difference in quality scores between "prestige" genres like Documentary or History and commercial ones like Animation ($p = 0.5967$), proving that quality is not limited to a single category.
- **Weak Link Between Ratings and Profit:** While a positive relationship exists, it is statistically weak. Higher-rated movies do not automatically guarantee high profits; ratings should be viewed as a secondary metric for brand reputation rather than a primary driver for financial investment.
- **Commercial Powerhouses:** Animation, Sci-Fi, and Adventure films generate the highest average worldwide profits. These genres demonstrate the strongest global appeal and represent the most reliable categories for sustainable revenue generation.
- **The Critical Importance of Timing:** The month of release is a major driver of profitability ($p < 0.05$). February, May, June, July, November, and December are peak months for profit, while "dump months" like January and September typically show much lower potential.
- **Domestic Success Predicts Global Reach:** We identified a strong positive correlation ($r \approx 0.73$) between domestic and worldwide gross. This makes domestic box-office performance a reliable leading indicator for a film's eventual global success.
- **Market Reach vs. Critical Acclaim:** Analysis suggests that a film's financial success is more heavily influenced by its genre selection and market reach than by its numeric critic rating alone.

**Key findings from our analysis include:**

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

## Recommendations

Based on our findings, we recommend the following strategic actions:

1. **Diversify for Quality, Focus for Profit:** Do not limit production to "prestige" genres to find high ratings. While any genre can achieve critical success, prioritize **Action, Adventure, and Animation** for financial sustainability.
2. **Strategic Release Timing:** Schedule major releases during high-profit windows (**May, June, July, or December**) and avoid the lower-performing "dump months" of January and September.
3. **Tiered Production Strategy:** Use a two-pronged approach:

- **Blockbusters:** High-budget Animation/Action for ROI.
- **Prestige Projects:** Low-budget History/Documentaries to build studio reputation and win awards without high financial risk.

## Team

- **Geoffrey Kemboi** | [LinkedIn](https://www.linkedin.com/in/geoffrey-kemboi-aiik-720345104/)
- **Peter Kiarie** | [LinkedIn](https://www.linkedin.com/in/geoffrey-kemboi-aiik-720345104/)
- **Natasha Wangare** | [LinkedIn](https://www.linkedin.com/in/geoffrey-kemboi-aiik-720345104/)
- **Samantha Jepkosgei** | [LinkedIn](https://www.linkedin.com/in/geoffrey-kemboi-aiik-72034)
- **Elvis Okeyo** | [LinkedIn](https://www.linkedin.com/in/geoffrey-kemboi-aiik-720345104/)
