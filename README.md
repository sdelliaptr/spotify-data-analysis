# 🎵 Spotify Data Analysis

Data analysis project exploring Spotify music popularity and audio characteristics using Python and Exploratory Data Analysis (EDA).

## 📌 About the Project

This project analyzes a dataset containing 114,000 Spotify tracks across different music genres.

The analysis focuses on exploring patterns in song popularity, audio characteristics, explicit content, and relationships between audio features.

The project follows several stages of the data analysis process, including data understanding, data cleaning, feature engineering, and exploratory data analysis (EDA).

## 🎯 Objectives

- Identify music genres with the highest average popularity.
- Explore the audio characteristics of songs with different popularity levels.
- Analyze the relationship between explicit content and song popularity.
- Analyze the relationship between explicit content and danceability.
- Explore relationships between Spotify audio features using correlation analysis.

## 📊 Dataset

The dataset consists of **114,000 Spotify tracks** across various music genres.

The dataset contains information about:

- Track and artist information
- Music genre
- Popularity
- Explicit content
- Danceability
- Energy
- Loudness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Tempo
- Duration

## 🔍 Analysis Process

### 1. Data Understanding

The dataset was explored to understand its structure and characteristics through:

- Dataset dimensions
- Data types
- Descriptive statistics
- Unique values
- Missing value identification
- Outlier detection
- Duplicate detection

### 2. Data Cleaning

Several preprocessing steps were performed:

- Handling missing values.
- Detecting and handling outliers using IQR Capping (Winsorization).
- Removing duplicate records.
- Normalizing categorical text by converting values to lowercase and removing unnecessary spaces.
- Verifying data types and data quality after cleaning.

### 3. Feature Engineering

Several new features were created to support the analysis:

- `duration_min` — converts track duration from milliseconds to minutes.
- `popularity_category` — categorizes songs into Low, Medium, and High popularity based on quantiles.
- `tempo_category` — categorizes tempo into Slow, Medium, and Fast based on quantiles.
- `explicit_encoded` — converts explicit values from boolean format into numerical values (0/1).

### 4. Exploratory Data Analysis

The analysis includes:

- Distribution of tracks across music genres.
- Top 10 genres based on the number of tracks.
- Top 10 genres based on average popularity.
- Distribution of song popularity.
- Popularity comparison between explicit and non-explicit songs.
- Danceability comparison based on explicit content.
- Audio feature profiles across popularity categories.
- Relationship between energy and danceability.
- Relationship between energy and valence.
- Correlation analysis between numerical audio features.

## 💡 Key Insights

- The dataset contains 114,000 tracks covering a wide range of music genres.
- Different music genres show differences in their average popularity.
- Songs with high popularity show different audio feature profiles compared with songs in lower popularity categories.
- Explicit and non-explicit songs show differences in their popularity and danceability distributions.
- `energy` and `loudness` show a strong positive correlation (r ≈ 0.76).
- `energy` and `acousticness` show a strong negative correlation (r ≈ -0.73).
- `valence` and `danceability` show a moderate positive relationship.
- `popularity` does not show a strong linear correlation with individual audio features, indicating that song popularity cannot be explained by audio characteristics alone.

## 🛠️ Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## 📁 Repository Structure

```text
spotify-data-analysis/
├── README.md
└── spotify-data-analysis.ipynb
