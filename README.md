<h1>IMDb Movie Analysis (2023) with Python</h1>

This project analyzes the 2023 IMDb movie dataset to uncover patterns and insights about movie performance, ratings, genre popularity, 
and other key features. Using Python and Pandas, we explore trends that shape the global film industry and support data-driven storytelling.


<h3>Objectives</h3>

- Clean and explore the 2023 IMDb movie dataset
- Perform univariate and bivariate analysis on numeric and categorical variables
- Visualize trends across genres, ratings, runtime, and release patterns
- Answer key questions about high-performing movies and industry patterns


<h3>Tools & Technologies</h3>

- **Python** – core programming language
- **Pandas** – for data wrangling and transformation
- **Matplotlib & Seaborn** – for data visualization
- **Jupyter Notebook** – for writing and presenting the analysis

<h3>Data Cleaning</h3>

Conducted in [`movie_analysis.ipynb`]

- Checked for and handled missing/null values
- Removed or corrected inconsistent genre and rating values
- Converted date and runtime fields to numeric for analysis
- Removed outliers where necessary (e.g., suspiciously low runtimes)


<h3>Exploratory Data Analysis (EDA)</h3>

**Univariate Analysis**
- Distribution of IMDb ratings
- Most common genres
- Movie count by year and runtime patterns

**Bivariate Analysis**
- Relationship between rating and runtime
- Top-rated genres vs. average runtime
- Ratings vs. vote count (popularity indicator)

**Advanced Insights**
- Genre-based rating comparisons
- Time trend of movies with 8+ ratings
- Does runtime affect IMDb ratings?

Example plot:

sns.boxplot(data=df, x='genre', y='imdb_rating')
plt.xticks(rotation=45)
plt.title('IMDb Ratings by Genre')


<h3>Insights</h3>

  - Drama was the most represented genre in R rated movies.
  - Movies with runtimes between 90–120 mins were the most common
  - Higher ratings tend to correlate with higher vote counts
  - Most movies were released mid-year (May–August) during winter, suggesting strategic timing
