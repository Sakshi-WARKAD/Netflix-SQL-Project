# Netflix Movies and TV Shows Data Analysis using SQL.

# Netflix Movies and TV Shows Data Analysis using SQL

## Project Overview
This project focuses on analyzing the Netflix Movies and TV Shows dataset using SQL to extract meaningful insights about the content available on the platform. By performing various SQL queries, we aim to understand trends, content distribution, popular genres, top countries, and more.

## Dataset
The dataset used for this analysis contains information about Netflix movies and TV shows. Key attributes include:
- **Title**: The name of the movie or TV show.
- **Director**: The director(s) of the movie or show.
- **Cast**: The actors/actresses featured in the content.
- **Country**: The country where the movie or show was produced.
- **Release Year**: The year the movie or show was released.
- **Duration**: The runtime of the movie or the number of seasons for a TV show.
- **Genre**: The category of the content, such as Drama, Documentary, or Comedy.
- **Ratings**: User ratings, if available.

The dataset was imported into an SQL database for analysis.

## Data Preparation
Before performing the analysis, several data cleaning steps were taken:
- **Handling missing data**: Missing values in key columns like `Director` and `Cast` were either filled with 'Unknown' or removed from specific queries based on the analysis context.
- **Formatting inconsistencies**: Ensured consistent formatting across columns such as `Release Year`, `Country`, and `Duration`.

## SQL Queries and Analysis
A variety of SQL queries were used to analyze the dataset and extract insights.

### Key Queries:
- **Content distribution by type**:
  ```sql
  SELECT type, COUNT(*) 
  FROM netflix_data 
  GROUP BY type;

