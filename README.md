<img width="1451" alt="Screenshot 2024-07-13 at 11 38 17 PM" src="https://github.com/user-attachments/assets/4cb0e35a-40f9-42bd-ac65-ed215f19fb7c">
Movie Recommendation System

This project builds a movie recommendation system using data from the TMDb (The Movie Database). It utilizes natural language processing techniques and cosine similarity to recommend movies based on their plot summaries, genres, keywords, cast, and crew.


-Dataset

Movies Data: tmdb_5000_movies.csv
Credits Data: tmdb_5000_credits.csv
Features Extracted

Extracted features include movie_id, title, overview, genres, keywords, cast, and crew.
Data preprocessing involved cleaning, transforming JSON strings, and feature selection.


-Methodology

1)Text Processing:

Converted JSON strings to lists of relevant features (genres, keywords, cast, crew).
Processed text data for overview, removing stopwords and special characters.

2)Feature Engineering:

Combined relevant features into a unified tags column.
Used CountVectorizer to transform tags into numerical vectors.

3)Similarity Calculation:

Applied cosine similarity on vectorized tags to compute movie similarities.

4)Recommendation:

Implemented a function to recommend movies based on user input.


-Technologies Used

Python, pandas, numpy for data manipulation.
scikit-learn for text processing and similarity calculations.
Streamlit for building the interactive recommendation interface.


-Files Included

app.py: Streamlit web app for user interaction.

movie_list.pkl: Serialized movie data after preprocessing.

similarity.pkl: Serialized cosine similarity matrix.
<img width="1448" alt="Screenshot 2024-07-13 at 11 39 36 PM" src="https://github.com/user-attachments/assets/fea02a39-e365-4a8f-8e09-6baac7f0550c">
<img width="1450" alt="Screenshot 2024-07-13 at 11 40 22 PM" src="https://github.com/user-attachments/assets/f671b8b0-2852-4f62-8f86-cb26eb2b2bf2">

