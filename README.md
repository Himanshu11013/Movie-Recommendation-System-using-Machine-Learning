Movie Recommendation and Filtering System
This project provides a K-Nearest Neighbors (KNN)-based movie recommendation system and a movie filtering system to recommend movies based on genre, cast, director, and year. The project uses a custom KNN algorithm to find similar movies and a filtering system to list top movies based on specific criteria.

Features
KNN Movie Recommendation:

Recommends similar movies based on genre, cast, and director.
Uses Euclidean distance to find the closest matches.
Outputs the top 10 similar movies.
Filter-based Movie Search:

Filter movies based on cast, director, genre, and year.
Outputs top 10 movies that match the criteria.
Allows flexible filtering with any combination of these fields.
Installation
Clone this repository:
git clone https://github.com/yourusername/movierecommendation
Install required libraries:
pip install pandas scikit-learn pickle-mixin
Usage
1. KNN Movie Recommendation
The KNN class processes movie data and predicts similar movies based on the provided movie name.
2. Movie Filtering
The Filter class allows you to filter movies based on a combination of cast, director, genre, and year.
Code Explanation
KNN Movie Recommendation
The KNN class preprocesses the movie dataset by expanding the genres and cast columns to fixed sizes (3 genres, 4 cast members).
It then calculates the Euclidean distance between the features of the selected movie and all other movies in the dataset.
The top 10 nearest movies are returned based on the calculated distances.
Movie Filter System
The Filter class allows dynamic filtering of movies based on any combination of cast, director, genre, and year.
The system tracks the number of matches for each movie and sorts them to return the top 10 most relevant movies.
Dataset
The dataset used should contain the following columns:

movie_name: Name of the movie
year: Year of release
genre: Genres of the movie (comma-separated)
cast: Cast members (comma-separated)
director: Director(s) of the movie
