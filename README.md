# Movies-ETL Project

## I used for this project:

Python, Anaconda Navigator, Jupyter Notebook 6.0.3, PostgreSQL, pgAdmin 4


## Project Overview

This project creates an automated pipeline that takes in new data, from Wikipedia data, Kaggle metadata, and the MovieLens rating data, then performs the appropriate transformations and loads the data to PostgreSQL database that has already been created by us.

For this analysis, we used the following breakdown:

1.	Write an ETL function to read three data files.
2.	Extract and transform the Wikipedia data.
3.	Extract and transform the Kaggle and rating data.
4.	Load the data to a PostgreSQL Movie Database.

## Results

### Write an ETL function to read three data files

This function takes the Wikipedia JSON, the Kaggle metadata and MovieLens csv files and creates three separate DataFrames.

### Extract and Transform the Wikipedia data

This function includes the following functions, filtering out the TV shows, consolidating the redundant data, removing the duplicates and formatting the Wikipedia data.

### Extract and Transform the Kaggle and rating data

For this function, we consolidated the redundant data, removed the duplicates, formatted and grouped the data.
The Kaggle and rating data were then merged with the Wikipedia movies DataFrame.

### Load the data to a PostgreSQL Movie Database

We loaded the movies_df  and MovieLens rating CSV files to a SQL database.

## Summary

The ETL(Extract-Transform-Load) function collected and cleaned movies’ data from different sources (Wikipedia JSON, Kaggle and ratings CSV files). It then transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the final users to apply the needed analysis.
