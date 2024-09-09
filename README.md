# 🎵 Content-Based Music Recommendation System 🎶

An intelligent system that recommends songs based on their intrinsic features, tailored to your musical preferences.

## 📚 Table of Contents
- [🎧 Overview](#-overview)
- [📊 Dataset](#-dataset)
- [📂 Project Structure](#-project-structure)
- [🚀 Installation](#-installation)

## 🎧 Overview
This repository contains a content-based music recommendation system developed using the "Top 10000 Songs on Spotify 1960-Now" dataset from Kaggle. The system recommends songs based on the similarity of features such as artist genres, danceability, energy, and more. By leveraging a TF-IDF vectorizer and cosine similarity, the system finds songs that closely match the user's input song, providing a personalized music experience.

## 📊 Dataset
The project uses the "Top 10000 Songs on Spotify 1960-Now" dataset, which includes songs released between 1960 and the present. This dataset is available on [Kaggle](https://www.kaggle.com/datasets/joebeachcapital/top-10000-spotify-songs-1960-now/data).

## 📂 Project Structure

The project is structured as follows:

1. **Data Exploration and Preprocessing:**
   - **Loading the Dataset:** Imported the "Top 10000 Songs on Spotify 1960-Now" dataset, which contains both textual and numerical features.
   - **Feature Selection:** Focused on key features like track name, artist name(s), artist genres, danceability, energy, acousticness, and more to use for recommendation purposes.
   - **Data Cleaning:** Handle missing values, normalize data, dropped duplicate entries and prepare it for modeling.

2. **Feature Engineering:**
   - **Textual Features:** Applied TF-IDF vectorization to textual features like artist genres and artist names separately to transform these into numerical vectors, enabling similarity calculations.
   - **Numerical Features:** Scaled numerical features such as danceability, energy, acousticness, etc., ensuring all features are on the same scale for accurate similarity measurements.
   - **Combining Features:** Combined the TF-IDF vectors and scaled numerical features into a single feature matrix. This matrix was then used for calculating similarities between songs.

3. **Similarity Calculation:**
   - **Cosine Similarity:** Implemented cosine similarity to measure the closeness between songs based on their feature vectors. This helped quantify how similar two songs are in terms of both their textual and numerical attributes.
   - **Recommendation Function:** Developed a custom function to recommend songs based on a given input song. This function uses cosine similarity to find the top 5 most similar songs.

4. **Model Evaluation and Testing:**
   - **Testing Recommendations:** Tested the recommendation system with various input songs, including popular tracks like "Love Story" and "You Belong With Me", to validate its performance.

## 🚀 Installation
To run this project, you need to have Python and the following libraries installed:

- numpy
- pandas
- scikit-learn

You can install these libraries using the following command:
```bash
pip install numpy pandas scikit-learn
```