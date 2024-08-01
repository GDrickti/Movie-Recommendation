# Movie-Recommendation

# Introduction

This project is a movie recommendation system that suggests movies based on user input. By leveraging cosine similarity and TF-IDF vectorization, the system analyzes movie metadata to find and recommend movies similar to the one provided by the user. This approach ensures that the recommendations are tailored to the user's tastes, based on various features of the movies.

# Workflow
### Data Collection:

Load the dataset containing movie metadata from a CSV file.

### Data Preprocessing:

Select relevant features for recommendation, such as genres, keywords, tagline, cast, and director.
Handle missing values by filling them with empty strings.

### Feature Engineering:

Combine selected features into a single string for each movie to create a unified text representation.

### Vectorization:

Use TfidfVectorizer to convert the combined text features into numerical values (TF-IDF vectors).

### Similarity Calculation:

Compute cosine similarity between all movie vectors to quantify how similar each pair of movies is.

### Recommendation Generation:

Take user input for their favorite movie.
Find the closest match to the input movie title from the dataset.
Retrieve the index of the matched movie and get similarity scores for all other movies.
Sort the movies based on similarity scores in descending order.
Display the top N recommended movies to the user.

# Results

When the user inputs their favorite movie, the system outputs a list of movies that are most similar to the input movie based on the combined features. The recommendations help users discover new movies that align with their preferences.

