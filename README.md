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
   - **Loading the Dataset:** Import the "Top 10000 Songs on Spotify 1960-Now" dataset.
   - **Feature Selection:** Analyze key features like artist genres, danceability, energy, and more.
   - **Data Cleaning:** Handle missing values, normalize data, and prepare it for modeling.

2. **Feature Engineering:**
   - **Textual Features:** Use TF-IDF vectorization for textual features like artist genres.
   - **Numerical Features:** Scale numerical features such as danceability and energy.
   - **Combining Features:** Merge all relevant features into a single feature matrix for similarity computation.

3. **Similarity Calculation:**
   - **Cosine Similarity:** Implement cosine similarity to measure the closeness between songs.
   - **Recommendation Function:** Build a function to recommend songs based on input criteria.

4. **Model Evaluation and Testing:**
   - **Testing Recommendations:** Test the recommendation system with various songs.
   - **Performance Evaluation:** Analyze the effectiveness of the recommendations.

## 🚀 Installation
To run this project, you need to have Python and the following libraries installed:

- numpy
- pandas
- scikit-learn

You can install these libraries using the following command:
```bash
pip install numpy pandas scikit-learn
```
