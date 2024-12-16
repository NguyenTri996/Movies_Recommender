# Movie Recommendation System

This project implements a **Movie Recommendation System** using the **MovieLens dataset**. It features two widely-used recommendation methods:

1. **Content-Based Filtering** using **TF-IDF Vectorization**.
2. **Collaborative Filtering** using **K-Nearest Neighbors (KNN)**.

---

## Features

### 1. Content-Based Filtering
- Utilizes **TF-IDF Vectorizer** to extract features from movie descriptions and genres.
- Calculates movie similarities based on textual metadata.
- Recommends movies similar to the user’s selected movie.

### 2. Collaborative Filtering
- Employs **K-Nearest Neighbors (KNN)** to find movies or users with similar rating patterns.
- Constructs a **sparse user-item utility matrix** using ratings data.
- Leverages **cosine similarity** to identify the closest matches and provide recommendations.

---

## Dataset
This project uses the [**MovieLens Dataset**](https://grouplens.org/datasets/movielens/), a popular dataset for recommendation systems. It includes:
- User ratings for movies.
- Metadata such as movie genres and IDs.
- Attributes essential for collaborative and content-based filtering techniques.

---

## Implementation

### Content-Based Filtering
1. Extracts movie genres from the dataset.
2. Applies **TF-IDF Vectorizer** to encode text-based information.
3. Computes similarity scores to recommend the top-`k` most similar movies to a given movie.

### Collaborative Filtering
1. Constructs a **user-item rating matrix** from user interaction data.
2. Applies **KNN-based collaborative filtering**:
   - Finds neighbors by analyzing user or movie rating patterns.
   - Recommends movies that are highly rated by similar users or have similar interactions.

---

## Technologies Used
- **Python** for implementation.
- **Scikit-learn** for machine learning utilities:
  - **TF-IDF Vectorizer** for feature extraction.
  - **NearestNeighbors** for collaborative filtering.
- **Pandas** and **NumPy** for efficient data manipulation.
- **Matplotlib** and **Seaborn** for data visualization.

---

