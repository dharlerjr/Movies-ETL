# Movies Extract, Transform, Load (ETL)

## Overview of Analysis


### Background


### Purpose

We have been tasked with preparing the following deliverables:

1. Deliverable 1: Write an ETL Function to Read Three Data Files
2. Deliverable 2: Extract and Transform the Wikipedia Data
3. Deliverable 3: Extract and Transform the Kaggle Data
4. Deliverable 4: Create the Movie Database

## Results

First, we created the `extract_transform_load()` function to read in three data files: a movies csv file from Kaggle, a movie ratings csv file from MovieLens, and a movies JSON file from Wikipedia. Next, we cleaned the Wikipedia dataset by performing various transformations such as removing TV shows with a list comprehension, extracting the IMDb ID for for each movie, and using regular expressions to clean columns containing monetary values, such as the box office and budget columns. We performed similar transformations to clean the Kaggle and MovieLens csv files. Once all three of the datasets were cleaned, we merged them into one movies_rating dataframe. Finally, using sqlalchemy, we loaded our transformed dataset a PostgresSQL database.
