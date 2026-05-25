# 🎬 Movie Recommender System

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Content--Based%20Filtering-success.svg)

## 📌 Overview
A Machine Learning-based Movie Recommender System that suggests similar movies based on a user's favorite film. This project uses the **TMDB 5000 Movies Dataset** to build a content-based filtering model. It analyzes movie metadata—such as genres, keywords, cast, and crew—to calculate the similarity between different films and recommend the closest matches.

## 🧠 How It Works (The Approach)
This system relies on **Content-Based Filtering**. 
1. **Data Preprocessing:** Merged the `movies` and `credits` datasets. Extracted and cleaned relevant features (Genres, Keywords, Cast, Director).
2. **Feature Engineering:** Combined the cleaned features into a single "tags" string for each movie. Apply stemming to reduce words to their root forms.
3. **Text Vectorization:** Used `CountVectorizer` (or TF-IDF) to convert the text data into vectors in a high-dimensional space.
4. **Similarity Calculation:** Applied **Cosine Similarity** to calculate the distance between the vectors. Movies with the smallest distance (highest cosine similarity score) are recommended.

## 🛠️ Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn, NLTK, ast
* **Environment:** Jupyter Notebook

## 📊 Dataset
The dataset used in this project is the [TMDB 5000 Movie Dataset](https://www.kaggle.com/tmdb/tmdb-movie-metadata) sourced from Kaggle. It contains metadata for around 5000 movies from The Movie Database (TMDb).

## 🚀 How to Run the Project Locally

**1. Clone the repository:**
```bash
git clone [https://github.com/](https://github.com/)[your-username]/[your-repo-name].git
cd [your-repo-name]
