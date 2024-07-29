[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/VaFOWmpj)


# Analysis of the Top 97 Movies on Rotten Tomatoes

## Introduction

This project analyzes the top 97 movies according to Rotten Tomatoes. The analysis aims to understand the distribution of ratings, the release years, actors involved, and other interesting patterns.

## Data Collection

The data was collected from various sources and compiled into three CSV files:
- `actors_list.csv`: Contains the list of actors with their IDs.
- `top_mov_actors.csv`: Contains the mapping of movies to actors.
- `top_movie.csv`: Contains the details of the top movies including their ranks, titles, release years, and ratings.

## Data Analysis

### 1. Distribution of Ratings

The Rotten Tomatoes ratings for the top 97 movies were analyzed to understand their distribution. Below is a summary of the key statistics:

- **Mean Rating:** 88.76%
- **Median Rating:** 92.00%
- **Standard Deviation:** 10.59%
- **Minimum Rating:** 42%
- **Maximum Rating:** 99%

### 2. Year of Release Analysis

The distribution of the years of release for the top 97 movies shows how the spread of top-rated movies spans different decades:

![Year of Release Distribution](docs/figures/year_wise_number_of_movies_released_bar_chart.png)

### 3. Actor Analysis

An analysis of the actors appearing in the top 97 movies reveals interesting patterns. Here are some key statistics:

- **Total Unique Actors:** 340
- **Most Frequent Actor:** Shirley MacLaine, Dustin Hoffman, Morgan Freeman, Clark Gable and Jack Nicholson (appeared in 3 movies)

![Most Frequent Actors](docs/figures/Most_Frequent_Actors.png)

### 4. Top 10 Movies

Here are the top 10 movies from the list, along with their Rotten Tomatoes ratings:

| Rank | Title                          | Year | Rating |
|------|--------------------------------|------|--------|
| #1   | Parasite                       | 2019 | 99%    |
| #2   | Casablanca                     | 1942 | 99%    |
| #3   | All About Eve                  | 1950 | 99%    |
| #4   | On the Waterfront              | 1954 | 99%    |
| #5   | Moonlight                      | 2016 | 98%    |
| #6   | Schindler's List               | 1993 | 98%    |
| #7   | It Happened One Night          | 1934 | 98%    |
| #8   | Rebecca                        | 1940 | 98%    |
| #9   | All Quiet on the Western Front | 1930 | 98%    |
| #10  | Sunrise                        | 1927 | 98%    |

## Conclusion

This analysis provides insights into the top-rated movies according to Rotten Tomatoes. The majority of these movies have very high ratings, reflecting their critical acclaim. The release years and actors also show a diverse range of movies, indicating that top-rated movies span across different times and include a variety of talents.

## Repository Structure

- `data/raw/`: Contains the dataset used for the analysis.
- `docs/figures/`: Contains the visualizations used in this markdown file.
- `notebooks/`: Contains the scripts used for data collection and analysis.
- `README.md`: This markdown file.

## How to Run the Analysis

To replicate the analysis:
1. Clone the repository.
2. Navigate to the `notebooks/` directory.
3. Run the data collection and analysis scripts as per the instructions in the `README.md` file.


# Software Requirements

## 1. Python
- Ensure Python 3.x is installed. Python 3.8 or later is recommended.

## 2. Package Management
- **pip**: Python’s package installer.
- **virtualenv**: To create isolated Python environments.
- **conda**: An alternative to virtualenv, comes with Anaconda distribution.

## 3. Data Handling and Analysis Libraries
- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical computing.
- **dask**: For parallel computing with larger-than-memory datasets.
- **polars**: A fast DataFrame library written in Rust, useful for performance-sensitive data manipulation.

## 4. Database Connectivity
- **SQLAlchemy**: For SQL database interaction.
- **psycopg2**: PostgreSQL adapter for Python.
- **pymysql**: MySQL connector for Python.
- **sqlite3**: SQLite database library included with Python.
- **pyodbc**: For connecting to various databases via ODBC.

## 5. Web Scraping and API Interaction
- **requests**: For making HTTP requests.
- **BeautifulSoup**: For parsing HTML and XML.
- **Scrapy**: A web scraping framework.
- **Selenium**: For web scraping with browser automation.
- **tweepy**: For interacting with the Twitter API.

## 6. Data Visualization
- **matplotlib**: For basic plotting.
- **seaborn**: For statistical data visualization.
- **plotly**: For interactive plots.
- **bokeh**: For interactive visualizations.

## 7. Data Serialization and File Formats
- **json**: For JSON file handling.
- **csv**: For CSV file handling.

## 8. Development Tools
- **VS Code**: A powerful code editor with Python support.
- **PyCharm**: A popular Python IDE.

## 9. Version Control
- **Git**: Version control system.
- **GitHub/GitLab/Bitbucket**: Hosting services for Git repositories.

## Installation Instructions
1. **Python Installation**:
    - Install the latest version of Python from [python.org](https://www.python.org/).
    - Verify installation: `python --version` or `python3 --version`.

2. **Package Installation**:
    - Use `pip` to install necessary packages:
      ```bash
      pip install pandas numpy dask polars sqlalchemy psycopg2 pymysql requests beautifulsoup4 scrapy selenium tweepy pyspark matplotlib seaborn plotly bokeh pyarrow fastparquet h5py airflow luigi prefect jupyterlab
      ```
    - Alternatively, use `conda`:
      ```bash
      conda install pandas numpy dask polars sqlalchemy psycopg2 pymysql requests beautifulsoup4 scrapy selenium tweepy pyspark matplotlib seaborn plotly bokeh pyarrow fastparquet h5py airflow luigi prefect jupyterlab
      ```

3. **Setting up Virtual Environment**:
    - Using `virtualenv`:
      ```bash
      pip install virtualenv
      virtualenv venv
      source venv/bin/activate  # On Windows use `venv\Scripts\activate`
      ```
    - Using `conda`:
      ```bash
      conda create --name myenv
      conda activate myenv
      ```



