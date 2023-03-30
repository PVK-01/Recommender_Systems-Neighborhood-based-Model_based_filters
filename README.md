# Recommender Systems: Neighborhood-based, Model-based filters
## Introduction, and Aim
• The entity to which the recommendation is provided is referred to as the user
• The product being recommended is an item.
The basic models for recommender systems works with two kinds of data:
- A User-Item interactions such as ratings (a user (you) provides ratings about a movie (item))
- B Attribute information about the users and items such as textual profiles or relevant keywords (deep representations about a user or item).

Models that use type A data are referred to as collaborative filtering methods, whereas models that use type B data are referred to as content-based methods. In this project, we will build a recommendation system using collaborative filtering methods.
In particular this project will look at Neighborhood based collaberative filtering and model based collaberative filters.

The project will contain the following parts:
- Neighborhood based collaberative filtering
- Model based collaberative filters
- Naive Collaberative filtering
- Peformance Comparision using ROC curves
- Recommend the top k items for a particular user

## Data Set
The dataset contains two csv files where one contains three columns one is movie id, other is user id and the last is the user rating for that particular movie.
The second CSV file conatins data about the movie, like what genre it is.

## Data selection for training
The data was trimmed into three different categories based on the distribution of the reviews for each movie.


## Neighborhood based collaberative filtering
## Suprise package in python was used for this project
The basic idea of collaborative filtering methods is that these unspecified ratings can be imputed because the observed ratings are often highly correlated across various users and items.
Computing pearson correlation coefficient between different users based on the common movies that they have reviewed. Then using this pearson correlation coefficient as simillarity measure between users and then predicting the rating for movies that were not rated by a specific user.
KNN colaberative filter was used as a eighborhood based collaberative filtering method and it was evaluated using CV with RMSE scores.

## Model based collaberative filters
Methods used:
- Latent factor based collaborative filtering
- NMF based collaborative filtering

#### Naive collaborative filtering method
#### Performance comparision between different models by RMSE and ROC curves

## Recommend the top k items for a particular user
Different models are used to predict the ratings and the movies with the highest k ratings are displayed for each user.