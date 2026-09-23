# Song Recommendation System

## Overview
This project builds a content-based song recommendation system. Given a song title, it recommends similar songs based on artist and genre. The dataset has 4,999 rows and 19 columns with song and audio features from Spotify.

## Steps
- Data cleaning: dropped rows with missing critical values, filled missing values with median or "unknown", fixed data types, removed duplicates
- Exploratory data analysis: looked at top genres, correlation between audio features, song popularity over the years, tempo, danceability, and energy distribution
- Recommendation model: combined artist name and genre into one text feature, used TF-IDF to turn it into vectors, then used cosine similarity to find similar songs
- Testing: tested the recommender with several songs from different genres (pop, rock, R&B) to check if the recommendations make sense

## Result
The recommender gives relevant results across different genres. For example, searching for a Pitbull song returns other Pitbull tracks with similar genres, and searching for a classic rock song returns other classic rock tracks.

## Tech Stack
Python, pandas, numpy, scikit-learn, seaborn, matplotlib
