# MOVIE SUCCESS ANALYSIS PROJECT 

## OVERVIEW 
This project explores the entertainment industry as there has been rapid evolving as major plays aim to produce original contents for streaming Platforms. In the project, we leveraged movie revenue data from Box office Mojo and IMDB database to analyze the movie ratings and characteristics.  The objective of this project is to conduct a comprehensive exploratory data analysis to identify patterns, relationships and factors contributing towards a movie success within the entertainment industry. The insights and findings gathered in this project can be transalted to actionable recommendations for companies within the industry. 

## Business Understanding 
A company plans to launch a new movie studio  but has no information on the performance of various movies at the box office. For the company to remain competitive, the company needs an understanding on best movie performances to make informed investment decisions. This project will explore historical data such as movie ratings, movie revenue and movie characteristics to guide the company on which movie studio to invest in and the type of films to produce. 

### Project Goal
Goal: To identify the key factors that drive movie box office success and to provide data driven insights to guide in the new movie studio and production venture. 

###  Business Questions 
1. which are the highest performing movie genres?
2. What is the impact of audience ratings on box office performance?
3. What are the key factors that determine movie success? factors such as runtime, genre and release timing 
4. How have the box office performance changed over the years? 

## Data Understanding and Analysis 

To achieve the goal of providing data driven insights on a new movie studio venture, two datasets were used in the project. 
1. bom.movie_gross.csv.gz — Box Office Mojo data with revenue information.
2. im.db — IMDB SQLite database containing movie information such as titles, genres, and ratings.

The two datasets are relevant in the project as :
1. BOM has revenue information for which revenue is one of our target variable
2. IMDB contains movie attributes which are more important for our objectives

First, the IMBD database contains multiple tables, however, only the movie_basics and movie_ratings contained relevant data for our analysis. The data on movie_ratings was good as did not contain duplicates or missing values but the movie_basics contained missing values which reqiuired cleaning by dropping rows or imputing . On the other hand, the Bom revenue data was messy and required cleaning such as dealing with missing values and duplicates. 

Eventually, we created a merge between the bom revenue dataset and the imbd datasets to generated a cleaned dataset for our analysis. The merge generated a data with 3109 rows and 13 columns. 

### Visualizations 
1. Top Performing Genres
![alt text](image-1.png)




