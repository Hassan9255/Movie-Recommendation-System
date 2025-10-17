# 🎬 Movie Recommendation System (MRS)

A **content-based Movie Recommendation System** built using **Python**, **Streamlit**, and **scikit-learn**.  
It recommends movies similar to the one selected by the user based on **movie genres, keywords, cast, and crew**.

🌐 **Live App:** [Movie Recommendation System on Streamlit](https://movie-recommender-system-tqugu9tqfxabyhv5p4kpmj.streamlit.app/)  
📊 **Dataset:** [TMDB Movie Metadata (Kaggle)](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

---

## 🚀 Features

- Uses **TF-IDF Vectorization** and **Cosine Similarity** for movie similarity.
- Recommends **top 10 most similar movies** to the selected title.
- Dynamically displays **movie posters** from the **TMDB API**.
- Simple, clean, and interactive **Streamlit web interface**.

---

## 🧠 How It Works

1. The dataset (`tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`) is loaded and merged in **`MRS.ipynb`**.
2. Extracts relevant features like **genres**, **keywords**, **cast**, and **crew**.
3. Combines them into a single text field called **`tags`**.
4. Applies **TF-IDF Vectorization** to convert text into numerical vectors.
5. Calculates **Cosine Similarity** to find related movies.
6. Saves the processed data into a **pickle file (`movie_data.pkl`)**.
7. The **Streamlit app (`app.py`)** uses this file to recommend and display movie posters.

---

## 🖥️ Project Structure

- MRS.ipynb # Data preprocessing and feature extraction
- app.py # Streamlit web app
- movie_data.pkl # Preprocessed movie dataset
- requirements.txt # Dependencies
- tmdb_5000_movies.csv # Movies dataset
- tmdb_5000_credits.csv # Credits dataset
- README.md # Project documentation
