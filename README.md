## MOVIE SUCCESS ANALYSIS PROJECT 

### Overview 
This project explores the entertainment industry as the industry has been evolving rapidly as major plays aim to produce original contents for streaming Platforms. In the project, we leveraged movie revenue data from Box office Mojo and IMDB database to analyze the movie ratings and characteristics. The objective of this project is to conduct a comprehensive exploratory data analysis to identify patterns, relationships and factors contributing towards a movie success within the entertainment industry. The insights and findings gathered in this project can be translated to actionable recommendations for companies within the industry.

## Business Understanding
A company plans to launch a new movie studio but has no information on the performance of various movies at the box office. For the company to remain competitive, the company needs an understanding on best movie performances to make informed investment decisions. This project will explore historical data such as movie ratings, movie revenue and movie characteristics to guide the company on which movie studio to invest in and the type of films to produce. The goal is to identify the key factors that drive movie box office success and to provide data driven insights to guide in the new movie studio and production venture.

### Business Questions 
1. Which are the highest performing movie genres?
2. What is the impact of audience ratings on box office performance?
3. What are the key factors that determine movie success? factors such as runtime, genre and release timing
4. How have the box office performance changed over the years?

## Data Understanding and Analysis

To achieve the goal of providing data driven insights on a new movie studio venture, two datasets were used in the project.

Box Office Mojo data with revenue information.i.e domestic and foreign gross - has revenue information for which revenue is one of our target variable

 IMDB SQLite database containing movie information such as titles, genres, and ratings.-IMDB contains movie attributes which are more important for our objectives
First, the IMBD database contains multiple tables, however, only the movie_basics and movie_ratings contained relevant data for our analysis. The data on movie_ratings was good as did not contain duplicates or missing values but the movie_basics contained missing values which reqiuired cleaning by dropping rows or imputing . On the other hand, the Bom revenue data was messy and required cleaning such as dealing with missing values and duplicates.

Eventually, we created a merge between the bom revenue dataset and the imbd datasets to generated a cleaned dataset for our analysis. The merge generated a data with 3109 rows and 13 columns

#Hypothesis Testing 
To determine whether there is a significant relationship between between movie genres and box office success, we conducted a Chi-Square Test of independence.

Null Hypothesis (H₀): There is no relationship between movie genre and box office success.

Alternative Hypothesis (H₁): There is a relationship between movie genre and box office succes

The results of the Chi-Square are shown below: Chi-Square Test Results

Chi2 Statistic: 736.6494756816546

p-value: 1.0623260172850567e-34

Degrees of Freedom: 321

From the results, the Chi-Square-Test has a statistic of 736.6 and a p- value of 1 0623260172850567e-34 which is below the significance level of 0.05. Therefore, we reject the null hypothesis and conclude that there is a significant relationship between movie genre and box office success.

