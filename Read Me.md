&nbsp;                                                                                                                                  **Exploratory Data Analysis of Amazon Prime TV-Shows and Movies**







**Dataset Description:**  



This dataset comprises of 2 types:



Amazon Prime Dataset (title.csv): This dataset contains metadata of movies and TV shows 	available on Amazon Prime Video, including variables related to title information, type of content, ratings (IMDB or TMDB), age certifications, released year, popularity and more.



Amazon Prime Cast Dataset (credits.csv): This dataset includes the information of Actors and Directors  who worked in Amazon Prime TV shows and movies. 



**Objective:**



To explore and analyze Amazon Prime’s catalog of movies and TV shows using key metadata such as genre, rating, popularity, age certification, and cast information. The goal is to uncover trends, patterns, and actionable insights for content strategy and audience engagement.



**Data Source:**



Scraped or collected from JustWatch.

Some fields may include external mappings (like actor-director-role relationships).	



**Variables Description:** 



Variable description of amazon\_data are as follows:



1\)  id- The unique identification for each title.



2\) title- Name of the Movie/TV-Show.



3\) type- Content type- either Movie or Show.



4\) description- Brief synopsis or summary of the title.



5\) release\_year- Year the Movie/Show was released.



6\) age\_certification- Age rating based on Regional Standard.



7\) runtime- Duration of the content (in minutes).



8\) genres- List of genres associated with title (e.g. Action, Drama, Comedy).



9\) production\_countries- List of countries where the content was produced.



10\) seasons- Number of seasons (only applicable for TV shows). NAN for Movies.



11\) imdb\_id- Unique identifier of the title on IMDB.



12\) imdb\_score- IMDB average rating score (Scale of 0 to 10).



13\) imdb\_votes- Number of IMDB votes received.



14\) tmdb\_score- TMDB average rating score.



15\) tmdb\_poplarity- TMDB popularity score.



Variable description of cast\_data are as follows:



1\) person\_id- The unique identifier for the name of Actor/Director in Amazon Prime.



2\) id- The unique identifier for the titles (in amazon\_data) linked with cast\_data.



3\) name- Name of the Actor/Director.



4\) character- The role/character played in the Movie/TV-Show.



5\) role- Classified name in the role of Actor/Director.



**Data Cleaning and Preprocessing:**



Replaced missing values in seasons for movies with 0.

List values were extracted and cleaned using custom function in genres and production\_countries.

Capitalized string values in type and role.

Converted imdb\_votes and seasons to integer types.

Removed unnecessary or duplicate rows in both the dataset.

Handle the missing values in columns like description, genres, production\_countries, imdb\_score, imdb\_votes and many more.



**Analysis Performed:** 



Distribution of Content type (Movies or TV-Shows).

Top performing genres by IMDB score or votes.

Trends over release year.

Correlation between imdb\_score and tmdb\_score.

Actors/Director gain more populartiy based on imdb\_votes.

Countries delivering best content in Amazon Prime.



**Key Insights:**



R rated Movies and TV-Shows domintes the age-certification.

Most contents are produced in US, followed by India and UK.

Genres like Drama, Comedy and Thriller are most common.

Documentary, Drama and Comedy genres score higher on IMDB.

A noticeable spike in releases between 2019-2021.

Positive correlation between imdb\_score and tmdb\_score.

Certain actors are linked with multiple genres and highly rated actors.



**Tools used in google colab:**



Libraries Used: 



1. pandas
2. numpy
3. matplotlib.pyplot
4. seaborn
5. plotly.express
6. warnings



Description:



* pandas, numpy for data manipulation.
* matplotlib, seaborn, plotly for visualization
* warnings to ignore warning messages.
* google colab for cloud based computing and analysis.



**Instructions for Use:**



Mount Google Drive if using external files.

Load the dataset into a pandas DataFrame.

Run the cleaning \& transformation cells.

Proceed with visualizations and insights.

Optionally export cleaned data or plots.



**Project Status:** 



Completed – Ready for storytelling, dashboarding, or business reporting.





