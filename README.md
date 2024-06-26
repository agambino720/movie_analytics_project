# movie_analytics_project

## Description
This project analyzed various movie datasets to generate business insights for a new movie studio. The analysis includes descriptive statistics and regression modeling to understand trends and patterns in the movie industry.

## Data Science Steps
1. **Data Loading and Cleaning:**
   - Loaded and cleaned the `movie_gross` dataset.
   - Loaded and cleaned data from the IMDb database, then merged it with the `movie_gross` data.
   - Loaded and cleaned the following datasets and merged them with the working dataframe:
     - `tmdb_movies`
     - `tn_movie_budgets`
     - `rt_movie_info`
2. **Analysis:**
   - Investigated the relationship between vote average and domestic gross.
   - Analyzed the relationship between runtime and domestic gross.
   - Studied the correlation between production budget and domestic gross.
   - Examined the relationship between production budget and average vote.
   - Identified which writers and directors had the best vote averages.
   - Analyzed the relationship between genre and domestic gross as well as genre and average vote.

## Summary of Findings and Recommendations

### Production Budget and Domestic Gross:
**Finding:** There is a strong positive correlation (0.71) between production budget and domestic gross. Adjusting the regression model by applying a log transformation and removing outliers confirmed that higher production budgets have a strong relationship with increased domestic gross revenue.
**Recommendation:** Allocate as much budget as possible to the production of new movies. Investing in higher production budgets can significantly enhance the chances of box office success, thereby ensuring higher domestic gross revenue.
**Explanation:** A larger production budget allows for higher quality production, better special effects, and the ability to attract top-tier talent including superior writers and directors, all of which contribute to a film’s box office success.

### Top-Rated Writers and Directors:
**Finding:** The top 5 writers and directors have significantly higher average votes compared to the overall averages. The top 5 writers have average votes ranging from 8.94 to 9.17, while the top 5 directors have average votes ranging from 8.90 to 9.23. This is in contrast to the overall average votes for writers (6.25) and directors (6.43). Additionally, all selected writers and directors had worked on at least 3 movies, ensuring consistent performance.
**Recommendation:** Prioritize hiring from among the top writers and directors. Recruiting talented writers like Beto Ribeiro, Natasa Kalinic Ahacic, Zeljko Luketic, Branko Istvancic, Yasmine Asha, and directors like Fan Li, Francois Lespes, Renjie, Georges Chamchoum, and Michael Burns can ensure creative excellence, resulting in higher audience engagement and appreciation of new movies.
**Explanation:** Recruiting top-rated writers and directors ensures high-quality storytelling and direction, which are crucial for audience satisfaction and critical acclaim. This, in turn, leads to improved commercial success.

### High-Grossing and Well-Received Genres:
**Finding:** Adventure, science fiction, and animation genres significantly outperform others in terms of average domestic gross, with revenues of 90.35 million, and $80.62 million respectively. Additionally, the short film genre is the most well-received by audiences with an average vote of 9.4, followed by game-show, documentary, news, biography, and music genres, which average between 7.1 and 7.3 out of 10.
**Recommendation:** Focus on producing movies in high-grossing genres while ensuring they are well-received by recruiting reputable writers and directors. Prioritize adventure, science fiction, and animation genres due to their higher average domestic gross revenues.
**Explanation:** Investing in high-grossing genres is likely to yield significant financial returns, potentially due to their popularity and broader appeal. Ensuring quality content within these genres by recruiting exceptional writers and directors and allocating adequate budgets will meet audience expectations, balancing financial goals with audience satisfaction.

## Repository Structure
- **data/**: Contains all the data files used in the project.
- **.gitignore**: Specifies files and directories to be ignored by git.
- **movie_analytics_project.ipynb**: Jupyter Notebook containing the data analysis and recommendations.
- **REAME.md**: Offers a detailed overview of the project including analysis insights and conclusions.

## Presentation
You can view the presentation of this project [here](https://docs.google.com/presentation/d/1qzzlDK3dgB4EjRu-NPncwXxS1F5_SCGlOMEQgSUlTeo/edit?usp=sharing).
