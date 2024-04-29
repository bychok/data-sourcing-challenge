![A modern workspace setup with a computer showing movie data dashboards](Movie_Data_Analysis.webp)

# Movie Data Analysis Project

This project fetches movie reviews from The New York Times API and detailed movie data from The Movie Database (TMDB). It merges the data for comprehensive analysis, offering insights into movie trends, genres, languages, and production countries.

## Table of Contents

- [Introduction](#introduction)
- [Technologies](#technologies)
- [Setup](#setup)
- [Features](#features)
- [Code Examples](#code-examples)
- [Status](#status)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The purpose of this project is to provide a comprehensive dataset that combines movie reviews with detailed movie metadata. This merged dataset can be used for various analyses, including sentiment analysis of reviews, genre popularity trends, and language diversity in films.

## Technologies

- Python 3.8+
- Pandas
- Requests
- Jupyter Notebook

## Setup

To run this project, install the required libraries using:

```bash
pip install pandas requests
```

Ensure you have API keys for both The New York Times and The Movie Database. Store these keys in your environment variables or a .env file for security.

## Features

- Fetch and parse movie reviews from The New York Times API.
- Retrieve detailed movie data from The Movie Database (TMDB).
- Clean and merge the data into a single DataFrame.
- Export the merged data to a CSV file for further analysis.
- Provide tools for basic data analysis within a Jupyter Notebook.

## Code Examples

To fetch data from The Movie Database:

```bash
import requests

def fetch_movie_data(title):
    url = f"https://api.themoviedb.org/3/search/movie?query={title}&api_key={tmdb_api_key}"
    response = requests.get(url)
    return response.json()
```

## Status

The project is in a functional state but continues to be open for expansion and refinement. Future updates may include advanced data analysis techniques and more interactive visualizations.

## Contributing

Contributions to the project are welcome! Please fork the repo, create a feature branch, and submit pull requests for review.

## License

This project is licensed under the MIT License.
