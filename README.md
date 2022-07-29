# Movies_ETL
Create An ETL Pipeline From Raw Data, Transform Data With Python,  And Load Data Into A SQL Database

## Project Overview
In this project, I created an automated pipeline for extracting data from both structured and unstructured files, transforming data with Python functions, building connection between Pyton and PostgreSQL, and loading cleaned dataset into the SQL database. 

### Purpose
- Create an ETL pipeline that transfers the raw data into a ready-to-analyze SQL database
- Extract data from different sources with Python
- Clean data with Pandas
- Filter and parse data with list comprehension and regular expression
- Load data to the PostgreSQL database

## Results
Before the transformation, the Wikipedia Movies JSON file has 7311 rows by 193 columns, the Kaggle movie metadata file has 45466 rows by 24 columns, and the ratings file has 26024289 rows by 4 columns.
After the transformation, Wikipedia Movies and Kaggle movie metadata files were cleaned and merged into the movies_df. Duplicate records were removed, duplicate columns were merged, and wrong data types were transformed. 

![movies_df](https://github.com/Wuyang080510/Movies_ETL/blob/main/movies_df.png)

The final movie_data database consists of two tables.
The movies table got data from movies_df. This table includes 6052 rows, each representing a unique movie title. The 31 columns have data related to movies' information like budget, revenue, runtime, director(s), actors, etc. 

![movies table](https://github.com/Wuyang080510/Movies_ETL/blob/main/movies_query.png)

The ratings table includes 26024289 records of viewers' ratings for disparate movies.  

![ratings table](https://github.com/Wuyang080510/Movies_ETL/blob/main/ratings%20query.png)
