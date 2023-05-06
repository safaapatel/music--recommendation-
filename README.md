# Music Recommendation System

Built a recommender sytem using the Spotify Dataset

Algorithms Used: 
      1. Decision Tree
      2. Decision Tree with Grid CV
      3. Random Forest

#Dataset
The Dataset is taken from Kaggle Website. The Data used in this was collected from Spotify’s Web API. This is basically a computer algorithm that Spotify has that can estimate various aspects of the audio file. More info on various attributes used in the dataset is found on this Spotify Developer page.


Installing
There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. The code should run with no issues using Python versions 3.*.


Project Tasks
Your project will be divided into the following tasks

I. Exploratory Data Analysis

First step is to explore the data you are working with for the project. Dive in to see what you can find. There are some basic, required questions to be answered about the data you are working with throughout the rest of the notebook. Use this space to explore, before you dive into the details.

II. ML Modelling

Before we start building a model for prediction. Let's first find the features which are highly correlated with Popularity feature and use them as feature variables that we will trained in the model. Next will be performing Feature Transformations. The steps followed are

      Object data of the artists with some numerical indicator that identify the artist.
      Eliminate Zero values from tempo columns and replace it
      Standardizing Instrumental Criteria with numeric values
      Using OneHotEncoder from SKlearn to create dummies
      Minmax Scaling for relevant features
      Target Scaling for Popularity Column
      
Below are a few models which I have attempted:

Decision Tree Regressor
Decision Tree with Grid Search CV
Random Forest Regressor (RF)
And the best accuracy is achieved by Decision Tree with Grid Search CV model

III. Neighbourhood Based Collaborative Filtering Recommendation

Building a recommendation system where it recommends similar songs for any given song.

In this project I have used Neighbourhood Collaborative Filtering using similarity metrics method. Calculated Manhattan Distance using all numerical features available in the dataset and find the neighbour songs which have relatively less distance.


File Structure
data folder contains the following:

data.csv: contains the songs data csv file
data_by_artist.csv: contains the artist data csv file
data_by_genres: contains the genres data csv file
data_by_year.csv: contains the Year Wise data csv file
data_w_genres.csv: contains the data with genres csv file
Spotify_Capstone_Project.ipynb  : Jupyter notebook with python codes


Results
Results are as follows:

The Mean Absolute Error and r2 score obtained from a test run using Decision Tree Regressor are 0.0792 and 74.896% respectively
The Mean Absolute Error and r2 score obtained from a test run using Decision Tree Regressor with Grid Search CV are 0.073 and 76.6% respectively
The Mean Absolute Error and r2 score obtained from a test run using Random Forest Regressor are 0.0758 and 74.683% respectively


The Best Accuracy is achieved using Decision Tree Regressor with Grid Search CV model



