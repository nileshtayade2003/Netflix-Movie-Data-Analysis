# Movie Data Analysis Project

## Overview
This project involves analyzing a dataset of movies to uncover insights about movie genres, popularity, vote averages, and release years. The dataset contains information about various movies, including their release dates, titles, popularity scores, vote counts, vote averages, and genres.

## Dataset
The dataset used in this project is named `mymoviedb.csv` and contains 9,827 rows and 9 columns. The columns include:
- **Release_Date**: The release date of the movie.
- **Title**: The title of the movie.
- **Overview**: A brief description of the movie.
- **Popularity**: A numerical score representing the movie's popularity.
- **Vote_Count**: The number of votes the movie received.
- **Vote_Average**: The average rating of the movie.
- **Original_Language**: The original language of the movie.
- **Genre**: The genre(s) of the movie.
- **Poster_Url**: A URL to the movie's poster.

## Data Cleaning and Preprocessing
1. **Handling Missing Values**: The dataset was checked for missing values, and no missing or null values were found.
2. **Removing Duplicates**: The dataset was checked for duplicate records, and no duplicates were found.
3. **Converting Data Types**: 
   - The `Release_Date` column was converted from an object to a datetime format, and only the year was extracted.
   - The `Genre` column was split into individual genres, and the dataframe was exploded to have one genre per row for each movie.
4. **Dropping Unnecessary Columns**: Columns such as `Overview`, `Original_Language`, and `Poster_Url` were dropped as they were deemed unnecessary for the analysis.
5. **Categorizing Vote_Average**: The `Vote_Average` column was categorized into four categories: `not_popular`, `below_avg`, `average`, and `popular`.

## Exploratory Data Analysis (EDA)
1. **Genre Distribution**: 
   - The most frequent genre in the dataset is **Drama**, which appears more than 14% of the time among 19 other genres.
   - A count plot was used to visualize the distribution of genres.

2. **Vote Average Distribution**:
   - The `Vote_Average` column was categorized, and the distribution of votes was visualized using a count plot.
   - **25%** of the dataset has movies with a `popular` vote, with **Drama** being the most popular genre among fans.

3. **Popularity Analysis**:
   - The movie with the highest popularity is **Spider-Man: No Way Home**, with genres **Action**, **Adventure**, and **Science Fiction**.
   - The movie with the lowest popularity is **The United States vs. Billie Holiday** and **Threads**, with genres **Music**, **Drama**, **History**, **War**, and **Science Fiction**.

4. **Release Year Analysis**:
   - The year **2020** has the highest number of movies released, as visualized by a histogram of the `Release_Date` column.

## Key Insights
1. **Most Frequent Genre**: **Drama** is the most frequent genre in the dataset.
2. **Highest Votes**: **25%** of the dataset has movies with a `popular` vote, with **Drama** being the most popular genre.
3. **Highest Popularity Movie**: **Spider-Man: No Way Home** has the highest popularity score.
4. **Lowest Popularity Movie**: **The United States vs. Billie Holiday** and **Threads** have the lowest popularity scores.
5. **Year with Most Movies**: The year **2020** has the highest number of movies released.

## Conclusion
This analysis provides valuable insights into the distribution of movie genres, popularity, and release years. The dataset is rich with information that can be further explored to uncover more trends and patterns in the movie industry.


## Requirements
- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`

