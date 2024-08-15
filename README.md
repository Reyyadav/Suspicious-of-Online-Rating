# Data Science Project: Fandango Movie Ratings Analysis

### Overview:
***When planning to watch a movie, you might wonder how trustworthy online reviews and ratings are, especially if the platform showing the ratings also profits from ticket sales. This project investigates whether Fandango's movie ratings in 2015 were biased towards higher ratings to drive ticket sales.***

### Goal:
The primary goal of this project is to determine if Fandango's ratings in 2015 exhibited a bias towards rating movies more favorably compared to other platforms like Metacritic, IMDb, and Rotten Tomatoes.

### Data Sources:
- fandango_scrape.csv: Contains Fandango's star ratings, true ratings, and vote counts for each movie.
- all_sites_scores.csv: Includes aggregate movie ratings from multiple platforms, such as Rotten Tomatoes, Metacritic, and IMDb.

### Part One: Understanding the Background and Data

### Data Overview:
The fandango_scrape.csv file includes the following columns:

- FILM: The movie title
- STARS: The star rating presented on Fandango
- RATING: The actual average score the movie obtained
- VOTES: The number of reviews the movie received

The all_sites_scores.csv file contains:

- FILM: The movie title
- RottenTomatoes: The Rotten Tomatoes critic score
- RottenTomatoes_User: The Rotten Tomatoes user score
- Metacritic: The Metacritic critic score
- Metacritic_User: The Metacritic user score
- IMDB: The IMDb user score
- Metacritic_user_vote_count: The number of user votes on Metacritic
- IMDB_user_vote_count: The number of user votes on IMDb

### Part Two: Exploring Fandango Displayed Scores versus True User Ratings

### Data Exploration:

- Load and inspect the data from fandango_scrape.csv.
- Explore the relationship between the popularity of a film (votes) and its rating by creating a scatterplot.
- Calculate the correlation between the columns STARS, RATING, and VOTES.

### Data Transformation:

- Extract the release year from the movie titles and analyze the distribution of movies per year.
- Identify the top 10 movies with the highest number of votes.
- Filter out movies with zero votes to focus on reviewed films.

### Visual Analysis:

- Create KDE plots to compare the distribution of Fandango's displayed ratings (STARS) versus the true user ratings (RATING).
- Quantify the discrepancy between displayed and true ratings by calculating and visualizing the difference.

### Part Three: Comparison of Fandango Ratings to Other Sites

### Rotten Tomatoes Analysis:

- Create scatterplots to explore the relationship between Rotten Tomatoes critic reviews and user reviews.
- Quantify and visualize the difference between critic and user ratings on Rotten Tomatoes.
- Identify the top 5 movies with the largest positive and negative differences between critic and user ratings.

### Metacritic Analysis:

- Analyze the relationship between Metacritic critic and user ratings using scatterplots.

### IMDb Analysis:

- Compare the vote counts on Metacritic versus IMDb to identify the most popular movies and any significant outliers.


### Results & Conclusion:
***The analysis reveals a pattern in Fandango's ratings that suggests a bias towards higher ratings, potentially to boost ticket sales. This conclusion is drawn from comparing Fandango's ratings to the true user ratings and the ratings from other platforms like Rotten Tomatoes, Metacritic, and IMDb. The project highlights the importance of being critical of online ratings, especially when the platform may have a vested interest in presenting movies more favorably.***

This project provides a comprehensive exploration of Fandango's ratings in 2015 and serves as a cautionary tale for moviegoers relying solely on platform ratings to make their viewing choices.
