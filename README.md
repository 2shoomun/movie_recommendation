# Movie Recommendation System

Welcome to the NLP driven movie recommendation system. This repository contains a content-based recommendation engine that suggests movies based on various metadata fields provided by the user, allowing flexible search options that cater to different interests and preferences.

## Project Overview

This project leverages machine learning techniques to build a versatile recommendation system, designed for movie enthusiasts. Users can enter any descriptive detail—such as a movie title, release year, character, or other metadata—and receive a curated list of similar movies. This flexibility enhances the user experience by allowing personalized exploration based on specific aspects of a film.

## Key Features

- **Flexible Metadata-Based Recommendations**: Input any information—title, genre, year, character, or keywords—to receive relevant recommendations.
- **Content-Based Filtering**: Uses various metadata to identify similar movies, providing meaningful results tailored to user input.
- **TF-IDF Vectorization**: Transforms movie metadata into structured data for nuanced recommendations.
- **Cosine Similarity Calculation**: Calculates similarity between movies to find the best matches based on the chosen metadata.
- **User-Friendly Interface**: Simple function for users to input any movie-related detail and receive recommendations.

## Data and Methodology

- **Dataset**: The system operates on the ["Top 10000 Popular Movies"](https://www.kaggle.com/datasets/omkarborikar/top-10000-popular-movies) dataset from Kaggle.
- **Data Preprocessing**: Manages missing values and prepares selected columns to ensure accurate recommendations.
- **Model**: Applies TF-IDF vectorization on multiple metadata fields, with cosine similarity providing the basis for similarity calculations.

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/2shoomun/movie_recommendation.git
   cd movie_recommendation
   ```

2. **Install Dependencies**:
   Ensure Python and the required libraries are installed. Use:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Notebook**:
   Open and execute `movie_recommendation_engine.ipynb` to preprocess data, build the model, and try out recommendations.

4. **Making Recommendations**:
   Use the recommendation function by inputting any movie-related information such as title, year, or character. The system will output a list of movies matching the specified criteria.

## Example

Here’s how the recommendation function can be used flexibly:

```python
recommend_movies("The Godfather")
recommend_movies("1972")
recommend_movies("Marlon Brando")
```

Each of these inputs will return movies relevant to the specified metadata, giving users control over their search.

## Technologies Used

- **Python** for programming
- **Pandas** for data processing
- **Scikit-learn** for TF-IDF vectorization and similarity measures
- **Jupyter Notebook** for interactive demonstration
