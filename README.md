# Movie Analytics Project

## Description
The Movie Analytics Project is designed to provide valuable business insights for a new movie studio by analyzing various movie datasets. This analysis utilized multiple data sources including movie gross data, IMDb data, TMDb movie data, TN movie budgets, and Rotten Tomatoes movie information. 

## Key Business Questions Answered:
1. **What is the relationship between production budget and domestic gross?**
   - Identifying how production investments translate into box office returns provides insights into budgeting strategies.
2. **Which writers and directors have the best vote averages?**
   - By identifying top-performing writers and directors, the studio can make informed hiring decisions to boost movie quality and audience appeal.
3. **How do different genres perform in terms of domestic gross and average votes?**
   - This analysis reveals which genres are most lucrative and well-received, guiding genre-specific production strategies.

## Stakeholders
The primary stakeholders for this project are:

**Head of the New Movie Studio:** Can use the insights to make informed decisions about which genres and types of films to produce, how much to invest into various films, as well as whom to consider hiring.

**Marketing Team:** Can utilize genre popularity data to create effective promotional strategies.

**Production Team:** Needs to understand which attributes of film production lead to increased success in the box office and ratings.

**Investors:** Interested in the financial costs, viability, and potential returns of investing in specific film genres.

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

**Visualization:**
This scatter plot showcases the relationship between the log-transformed production budget and the log-transformed domestic gross revenue, with a regression line fitted to the data. The data points represent individual movies, and the red line represents the fitted regression model after removing outliers.

![image](https://github.com/agambino720/movie_analytics_project/assets/135170174/ed883a2c-2a2f-4ac7-8262-5d896ef2a94e)


### Top-Rated Writers and Directors:
**Finding:** The top 5 writers and directors have significantly higher average votes compared to the overall averages. The top 5 writers have average votes ranging from 8.94 to 9.17, while the top 5 directors have average votes ranging from 8.90 to 9.23. This is in contrast to the overall average votes for writers (6.25) and directors (6.43). Additionally, all selected writers and directors had worked on at least 3 movies, ensuring consistent performance.

**Recommendation:** Prioritize hiring from among the top writers and directors. Recruiting talented writers like Beto Ribeiro, Natasa Kalinic Ahacic, Zeljko Luketic, Branko Istvancic, Yasmine Asha, and directors like Fan Li, Francois Lespes, Renjie, Georges Chamchoum, and Michael Burns can ensure creative excellence, resulting in higher audience engagement and appreciation of new movies.

**Explanation:** Recruiting top-rated writers and directors ensures high-quality storytelling and direction, which are crucial for audience satisfaction and critical acclaim. This, in turn, leads to improved commercial success.

**Visualization:** 
This histogram highlights that the top 5 writers have significantly higher average votes compared to the overall average for all writers. This suggests that the top writers consistently produce work that is much better received by audiences.

![image](https://github.com/agambino720/movie_analytics_project/assets/135170174/bdb25a7a-cb62-460f-b37f-b540331012b7)

**Visualization:** 
This histogram demonstrates that the top 5 directors have significantly higher average votes compared to the overall average for all directors. This showcases that the top directors also consistently produce work that is much better received by audiences.

![image](https://github.com/agambino720/movie_analytics_project/assets/135170174/fa6a757c-b9fd-46b7-b164-90dc17ccbc13)


### High-Grossing and Well-Received Genres:
**Finding:** Adventure, science fiction, and animation genres significantly outperform others in terms of average domestic gross, with revenues of 90.35 million, and $80.62 million respectively. Additionally, the short film genre is the most well-received by audiences with an average vote of 9.4, followed by game-show, documentary, news, biography, and music genres, which average between 7.1 and 7.3 out of 10.

**Recommendation:** Focus on producing movies in high-grossing genres while ensuring they are well-received by recruiting reputable writers and directors. Prioritize adventure, science fiction, and animation genres due to their higher average domestic gross revenues.

**Explanation:** Investing in high-grossing genres is likely to yield significant financial returns, potentially due to their popularity and broader appeal. Ensuring quality content within these genres by recruiting exceptional writers and directors and allocating adequate budgets will meet audience expectations, balancing financial goals with audience satisfaction.

**Visualization:**
This histogram showcases the average domestic gross revenue of the top 10 individual genres by domestic gross. The genres on the left, such as adventure, science fiction, and animation, show significantly higher average domestic gross revenues This indicates that these genres tend to perform better financially.

![image](https://github.com/agambino720/movie_analytics_project/assets/135170174/5668d966-af7f-4f57-a177-c466e00a6146)

**Visualization:**
This histogram shows the average votes of the top 10 genres by average vote. Short films have a notably higher average vote compared to the other genres. The remaining top 9 genres, including: game-show, documentary, news, biography, music, history, talk-show, sport, and war, have relatively similar average votes.

![image](https://github.com/agambino720/movie_analytics_project/assets/135170174/50138f8d-daa1-423c-9514-27ada5d5981b)


## Repository Structure
- **data/**: Contains all the data files used in the project.
- **.gitignore**: Specifies files and directories to be ignored by git.
- **movie_analytics_project.ipynb**: Jupyter Notebook containing the data analysis and recommendations.
- **REAME.md**: Offers a detailed overview of the project including analysis insights and conclusions.

## Presentation
You can view the presentation of this project [here](https://docs.google.com/presentation/d/1qzzlDK3dgB4EjRu-NPncwXxS1F5_SCGlOMEQgSUlTeo/edit?usp=sharing).
