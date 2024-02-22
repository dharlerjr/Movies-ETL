# Movies Extract, Transform, Load (ETL)

## Overview of Analysis

### Background

AmazingPrimeVideo is a fictional streaming service that allows customers to stream movies and tv shows. The AmazingPrimeVideo team wants to expand their movie catalog by developing an algorithm to predict which low-budget movies will become popular. To do so, the company has sponsored a Hackathon in which participants will build their own algorithm to try and predict the popular movies. However, the participants will need a sufficient dataset for to develop and test their algorithms.

### Purpose

We have been tasked with preparing the dataset for the Hackathon participants. Our task has been divided into the following four deliverables:

1. Deliverable 1: Write an ETL Function to Read Three Data Files
2. Deliverable 2: Extract and Transform the Wikipedia Data
3. Deliverable 3: Extract and Transform the Kaggle Data
4. Deliverable 4: Create the Movie Database

## Results

First, we created the `extract_transform_load()` function to read in three data files: a movies csv file from Kaggle, a movie ratings csv file from MovieLens, and a movies JSON file from Wikipedia. Next, we cleaned the Wikipedia dataset by performing various transformations such as removing TV shows with a list comprehension, extracting the IMDb ID for for each movie, and using regular expressions to clean columns containing monetary values, such as the box office and budget columns. We performed similar transformations to clean the Kaggle and MovieLens csv files. Once all three datasets were cleaned, we merged them into one dataframe. Finally, using sqlalchemy, we loaded our final dataframe into a PostgresSQL database.
