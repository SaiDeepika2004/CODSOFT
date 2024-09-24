# Movie Rating Prediction with Python

![image](https://github.com/user-attachments/assets/b1dc27c1-fd1e-48f9-b582-0dd7925e2e42)


## Table of Contents
- [Project Overview](#project-overview)
- [Business Understanding](#business-understanding)
- [Objectives](#objectives)
- [Data Understanding](#data-understanding)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Modeling](#modeling)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)
- [Next Steps](#next-steps)

## Project Overview 
The **Movie Rating Prediction** project aims to analyze a dataset containing information about Indian movies and build a machine learning model to predict movie ratings. The dataset includes variables such as movie name, release year, duration, genre, rating, votes, director, and the leading actors. This analysis provides valuable insights to stakeholders in the film industry for data-driven decision-making.

## Business Understanding
The film industry relies heavily on understanding what drives a movie's success. Predicting movie ratings with accuracy can assist in making informed decisions about movie production, casting, genres, and marketing strategies, enhancing a movie's overall success.

## Objectives
- **Build a Predictive Model**: Create a machine learning model capable of predicting movie ratings based on the dataset's features. This regression task aims to estimate movie ratings using various input variables.
- **Identify Key Factors**: Determine which factors (e.g., genre, director, actors) have the most influence on movie ratings.
- **Actionable Insights**: Provide industry stakeholders with insights to guide decisions on movie production, casting, and marketing strategies.

## Data Understanding
The dataset used for this project is from Kaggle: [IMDb India Movies](https://www.kaggle.com/datasets/adrianmcmahon/imdb-india-movies).

Key columns in the dataset:
- `Name`: Movie name
- `Year`: Release year of the movie
- `Duration`: Movie runtime (in minutes)
- `Genre`: Movie genre
- `Rating`: IMDb rating of the movie
- `Votes`: Number of votes received by the movie
- `Director`: Movie director
- `Actor 1`, `Actor 2`, `Actor 3`: Main actors in the movie

## Exploratory Data Analysis (EDA)
Key insights from the EDA include:
- Rating Distribution
- Top 10 Directors with the Most Movies Directed
- Top 10 Actors with the Most Movie Appearances
- Top 10 Directors with the Highest-Rated Movies
- Top 10 Highest-Rated Movie Genres
- Top 10 Years with the Highest Average Ratings
- Duration vs. Rating Analysis

## Modeling
Three machine learning models were explored:
1. **Baseline Model**: Linear Regression
2. **Second Model**: Gradient Boosting Regressor


### Key Features
The most influential features in predicting movie ratings:
- `Year`: The release year of the movie
- `Votes`: Number of votes received
- `Duration`: The movie's runtime

## Recommendations
- **Year**: Monitor release year trends to align production with successful movie patterns.
- **Votes**: Encourage user engagement and reviews to enhance reliability in ratings.
- **Duration**: Consider audience preferences for movie length when planning releases.
- **Collaboration**: Work with prominent industry figures to increase movie success.
- **Genres**: Invest in high-performing genres such as History and Romance.
- **Duration vs. Ratings**: No clear correlation, suggesting runtime should be tailored to the story rather than aiming for specific lengths.
- **Critical Acclaim**: Strive for critical praise and positive reviews for higher ratings.

## Conclusion
This project has successfully provided a predictive model for movie ratings along with insights into factors that influence them. By leveraging these findings, the film industry can optimize decision-making related to movie production, casting, and marketing. The most important factors identified were the year of release, the number of votes, and the movie's duration.

## Next Steps
- **Model Refinement**: Further enhance the predictive model by exploring advanced machine learning techniques and fine-tuning hyperparameters.
- **Feature Engineering**: Investigate new feature engineering methods to improve model performance.
- **User Reviews Analysis**: Include sentiment analysis of user reviews to better understand audience reactions and preferences.
- **Real-time Data Updates**: Develop mechanisms for incorporating real-time data to keep the model relevant with current trends and new releases.
