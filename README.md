# Project Overview

This project applies advanced data science and machine learning techniques to a large commercial dataset to investigate the factors driving modern music popularity. The core objective is to develop a predictive model to forecast a song's streaming success based on its audio features, release metrics, and chart performance. This study combines exploratory data analysis (EDA) with supervised learning to extract statistical insights into the complex dynamics of the music industry.

# Research Question
Can we effectively predict the streaming popularity of a song, and what are the key statistical and acoustic features (e.g., danceability, energy, release timing) that significantly contribute to or correlate with that success?

# Methodology & Analysis
The analysis follows a standard quantitative research pipeline:

## Data Acquisition and Cleaning:
The raw Spotify 2023 dataset (N=953 songs, 24 features) was imported and cleaned in Python.

The crucial streams column was converted to a uniform numeric format to serve as the target variable for prediction. Missing values (NAs) were handled systematically.

## Exploratory Data Analysis (EDA):

Visualizations were generated using Matplotlib and Seaborn to analyze the distribution of song features (e.g., BPM, key, acousticness) and their initial correlations with the target variable (streams).

A comparative analysis was performed across different streaming platforms (Spotify, Apple Music, Deezer) to identify market-specific popularity trends, which revealed divergent patterns and the influence of platform algorithms and regional preferences.

## Feature Impact Case Study (Taylor Swift):

A focused time-series analysis was conducted on a high-stream artist (Taylor Swift) post-2018 to determine if major events, such as seasonal award shows, correlate with quantifiable spikes in streaming volume. The analysis showed that the artist's streams remained high and stable across the study period.

## Machine Learning Model:

A Random Forest Regressor model was employed to predict the magnitude of song streams. Random Forest was chosen for its ability to capture non-linear relationships and provide strong feature importance rankings. (Note: The model implementation is contained within the notebook.)

## Key Findings & Statistical Implications
While predictive modeling offers insight, the study concluded that accurately predicting future hit songs remains inherently complex and elusive.

Multifactorial Success: Success is driven by a complex interplay between quantitative features (e.g., in-playlist counts) and qualitative variables like audience taste, social media trends, and marketing campaigns.

Acoustic Features: Initial EDA confirmed some acoustic attributes correlate with popularity, but the model emphasized the significant predictive power of metrics reflecting initial market traction (e.g., in_spotify_charts and in_spotify_playlists).

### Technologies Used
Programming Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (RandomForestRegressor)

Environment: Jupyter Notebook / Google Colab
