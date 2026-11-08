# Netflix Data Science Analysis & Prediction

This project analyzes Netflix title data to understand content patterns, viewer trends, and possible future predictions. It combines data cleaning, exploratory data analysis, recommendation logic, and forecasting to turn raw entertainment metadata into useful insights.

## Project Overview

The workflow includes:

- Cleaning and preparing raw Netflix dataset files
- Performing exploratory data analysis (EDA) on title types, countries, ratings, and release trends
- Building a content-based recommendation system
- Analyzing release and popularity patterns for trend prediction
- Producing a reusable notebook-based pipeline for future experimentation

## Repository Structure

```text
Netflix Data Science Analysis & prediction/
├── data/
│   ├── raw_data/
│   │   └── Dataset (1).csv
│   └── clean_data/
│       └── clean_dataset.csv
├── notebook/
│   ├── data_cleaning.ipynb
│   ├── netflix_data_analysis.ipynb
│   ├── netflix_recommendation_system.ipynb
│   └── trend_prediction.ipynb
├── outputs/
│   └── figures/               # Exported charts from the analysis notebooks
├── screenshots/
│   └──                     # Selected chart snapshots for quick reference
├── README.md
├── requerements.txt
```

## Outputs and Screenshots

- The saved charts from the analysis and trend-prediction notebooks are exported to [outputs/figures/](outputs/figures/).
- Selected visual results are also available in [screenshots/](screenshots/) for quick review.
- Save future project artifacts (charts, tables, forecasts, and recommendation examples) in `outputs/`, using descriptive filenames.
- Keep screenshots of important notebook results and visualizations in `screenshots/`. The cleaned dataset remains in `data/clean_data/` because it is an input to the analysis notebooks.

## Dataset

The project uses a Netflix dataset containing metadata such as:

- show_id
- type (Movie / TV Show)
- title
- director
- country
- date_added
- release_year
- rating
- duration
- listed_in

The cleaned dataset is stored in:

- [data/clean_data/clean_dataset.csv](data/clean_data/clean_dataset.csv)

The original unprocessed dataset is available in:

- [data/raw_data/Dataset (1).csv](data/raw_data/Dataset%20(1).csv)

## Notebooks

### 1. Data Cleaning

[notebook/data_cleaning.ipynb](notebook/data_cleaning.ipynb)

This notebook handles:

- loading the raw dataset
- checking missing values and duplicates
- removing invalid or inconsistent records
- preparing a clean dataset for analysis

### 2. Netflix Data Analysis

[notebook/netflix_data_analysis.ipynb](notebook/netflix_data_analysis.ipynb)

This notebook focuses on exploratory insights, including:

- distribution of movies vs. TV shows
- countries contributing the most content
- year-wise release patterns
- ratings and category trends
- content duration analysis

### 3. Recommendation System

[notebook/netflix_recommendation_system.ipynb](notebook/netflix_recommendation_system.ipynb)

This notebook builds a content-based recommendation engine using features such as:

- title
- type
- director
- country
- genre
- release year
- rating

It uses TF-IDF vectorization and cosine similarity to recommend titles similar to a selected title.

### 4. Trend Prediction

[notebook/trend_prediction.ipynb](notebook/trend_prediction.ipynb)

This notebook explores forecasting and regression-based approaches to:

- analyze release-year patterns
- estimate future content trends
- evaluate predictive performance using simple machine learning models

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- Jupyter Notebook

## Setup

1. Clone the repository.
2. Create a virtual environment.
3. Install dependencies:

```bash
pip install -r requerements.txt
```

If you want to install the main packages manually instead:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels jupyter
```

## Run the Project

Open the notebooks in Jupyter Notebook or JupyterLab and run them in order:

```bash
jupyter notebook
```

Then open:

1. [notebook/data_cleaning.ipynb](notebook/data_cleaning.ipynb)
2. [notebook/netflix_data_analysis.ipynb](notebook/netflix_data_analysis.ipynb)
3. [notebook/netflix_recommendation_system.ipynb](notebook/netflix_recommendation_system.ipynb)
4. [notebook/trend_prediction.ipynb](notebook/trend_prediction.ipynb)

## Expected Outcomes

This project helps answer questions such as:

- What type of content dominates Netflix?
- Which countries contribute the most titles?
- Which titles are similar to each other?
- What can historical trends suggest about future content growth?

## License

This project is intended for educational and research purposes.

## Note

The repository uses the filename `requerements.txt`, which is a common misspelling of `requirements.txt`. If needed, you may rename it to `requirements.txt` for standard Python convention.
