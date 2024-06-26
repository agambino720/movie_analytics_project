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
3. **Findings:**
   - Found a strong relationship between production budget and domestic gross.
   - Identified the top 5 writers and directors by average vote.
   - Determined which genres had the highest average domestic gross and highest average votes.

## Repository Structure
- **data/**: Contains all the data files used in the project.
- **.gitignore**: Specifies files and directories to be ignored by git.
- **movie_analytics_project.ipynb**: Jupyter Notebook containing the data analysis and recommendations.
- **REAME.md**: Offers a detailed overview of the project including analysis insights and conclusions.

## Presentation
You can view the presentation of this project [here](https://docs.google.com/presentation/d/1qzzlDK3dgB4EjRu-NPncwXxS1F5_SCGlOMEQgSUlTeo/edit?usp=sharing).
