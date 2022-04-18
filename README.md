# Movies-ETL

## Purpose
Create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. You’ll need to refactor the code from this module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database

This new assignment consists of four technical analysis deliverables. You will submit the following:

- Deliverable 1: Write an ETL Function to Read Three Data Files
    - Write a function that reads in the three data files and creates three separate DataFrames
- Deliverable 2: Extract and Transform the Wikipedia Data
    - Extract and transform the Wikipedia data so you can merge it with the Kaggle metadata. While extracting the IMDb IDs using a regular expression string and dropping duplicates, use a try-except block to catch errors.
- Deliverable 3: Extract and Transform the Kaggle data
    - Extract and transform the Kaggle metadata and MovieLens rating data, then convert the transformed data into separate DataFrames. Then, you’ll merge the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. Finally, you’ll merge the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df
- Deliverable 4: Create the Movie Database
    - Add the movies_df DataFrame and MovieLens rating CSV data to a SQL database.  Outputs are two tables in an SQL database with the following values:
        - ![Movie Queries](Resources/movies_query.png)
        - ![Rating Queries](Resources/ratings_query.png)