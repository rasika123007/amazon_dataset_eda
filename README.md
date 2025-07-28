# Exploratory Data Analysis of Amazon Prime Shows and Movies

This project performs Exploratory Data Analysis (EDA) on a dataset of TV shows and movies available on Amazon Prime Video. Using Python libraries such as Pandas, Matplotlib, Seaborn and Plotly, the project explores key aspects of the platform's content library including:

* Content types (TV Shows vs Movies)
* Genre distribution
* Country-wise availability
* Release year trends
* Age ratings and parental guidance
* IMDB ratings and Votes
* TMDB rating and votes
* Duration and runtime patterns

The main goal is to extract insights and patterns that help understand how Amazon Prime curates and distributes its content globally. The analysis is visualized through clear and informative charts for better interpretability.

## Objective:

To explore and analyze Amazon Prime’s catalog of movies and TV shows using key metadata such as genre, rating, popularity, age certification, and cast information. The goal is to uncover trends, patterns, and actionable insights for content strategy and audience engagement.


## Set up Instructions:

1.	Mount Google Drive if using external files.
2.	Load the dataset into a pandas DataFrame.
3.	Run the cleaning & transformation cells.
4.	Proceed with visualizations and insights.
5.	Optionally export cleaned data or plots.

## Data Source:
Scraped or collected from JustWatch.
Some fields may include external mappings (like actor-director-role relationships).

## Variables Description:

Variable description of amazon_data are as follows:

1) id- The unique identification for each title.
2) title- Name of the Movie/TV-Show.
3) type- Content type- either Movie or Show.
4) description- Brief synopsis or summary of the title.
5) release_year- Year the Movie/Show was released.
6) age_certification- Age rating based on Regional Standard.
7) runtime- Duration of the content (in minutes).
8) genres- List of genres associated with title (e.g. Action, Drama, Comedy).
9) production_countries- List of countries where the content was produced.
10) seasons- Number of seasons (only applicable for TV shows). NAN for Movies.
11) imdb_id- Unique identifier of the title on IMDB.
12) imdb_score- IMDB average rating score (Scale of 0 to 10).
13) imdb_votes- Number of IMDB votes received.
14) tmdb_score- TMDB average rating score.
15) tmdb_poplarity- TMDB popularity score.
    
Variable description of cast_data are as follows:

1) person_id- The unique identifier for the name of Actor/Director in Amazon Prime.
2) id- The unique identifier for the titles (in amazon_data) linked with cast_data.
3) name- Name of the Actor/Director.
4) character- The role/character played in the Movie/TV-Show.
5) role- Classified name in the role of Actor/Director.
   
## Data Cleaning and Preprocessing:
* Replaced missing values in seasons for movies with 0.
* List values were extracted and cleaned using custom function in genres and production_countries.
* Capitalized string values in type and role.
* Converted imdb_votes and seasons to integer types.
* Removed unnecessary or duplicate rows in both the dataset.
* Handle the missing values in columns like description, genres, production_countries, imdb_score, imdb_votes and many more.
  
## Analysis Performed:
* Distribution of Content type (Movies or TV-Shows).
* Top performing genres by IMDB score or votes.
* Trends over release year.
* Correlation between imdb_score and tmdb_score.
* Actors/Director gain more populartiy based on imdb_votes.
* Countries delivering best content in Amazon Prime.
  
## Key Insights:
* R rated Movies and TV-Shows domintes the age-certification.
* Most contents are produced in US, followed by India and UK.
* Genres like Drama, Comedy and Thriller are most common.
* Documentary, Drama and Comedy genres score higher on IMDB.
* A noticeable spike in releases between 2019-2021.
* Positive correlation between imdb_score and tmdb_score.
* Certain actors are linked with multiple genres and highly rated actors.
  
# Tools used in google colab:

Libraries Used:

1.	pandas
2.	numpy
3.	matplotlib.pyplot
4.	seaborn
5.	plotly.express
6.	warnings
   
## Description:

•	pandas, numpy for data manipulation.
•	matplotlib, seaborn, plotly for visualization
•	warnings to ignore warning messages.
•	google colab for cloud based computing and analysis.

## Instructions for Use:

1.	Mount Google Drive if using external files.
2.	Load the dataset into a pandas DataFrame.
3.	Run the cleaning & transformation cells.
4.	Proceed with visualizations and insights.
5.	Optionally export cleaned data or plots.
   
## Project Status:

Completed – Ready for storytelling, dashboarding, or business reporting.

## Author:
**Rasika Dilip Mundaye**  

email-address: rasika123m@gmail.com

LinkedIn: www.linkedin.com/in/rasika-mundaye-939117200




