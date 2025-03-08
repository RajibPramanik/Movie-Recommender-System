# Movie-Recommender-System
## Overview 
This is a content-based movie recommendation system that suggests similar movies based on user input.

## Dataset
The system uses TMDB 5000 Movies Dataset, which consists of two files:

- tmdb_5000_movies.csv – Contains movie details such as title, overview, genres, and keywords.
- tmdb_5000_credits.csv – Contains cast and crew information.

## Approach
1. Data Preprocessing
- Merging movie details with credits.
- Extracting useful features like genres, keywords, cast, and crew.
- Converting text data into a structured format.
  
2. Feature Engineering
- Combining relevant information into a single "tags" column.
- Applying stemming to normalize words.
- Converting text data into numerical vectors using TF-IDF or CountVectorizer.

3. Similarity Calculation
- Using cosine similarity to measure the closeness between movies.
- Sort and retrieving the top recommended movies.


## Files in the Project
- movie-recommender-system.ipynb → Jupyter Notebook containing the implementation.
- tmdb_5000_movies.csv & tmdb_5000_credits.csv → Dataset files.
- movies.pkl → Processed movie data stored as a pickle file.
- movie_dict.pkl → Dictionary for fast movie lookup.
- similarity.pkl → Precomputed similarity matrix for quick recommendations.


