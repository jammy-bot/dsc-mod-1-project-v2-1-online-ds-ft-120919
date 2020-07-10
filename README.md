# Module 1 Final Project
![arms holding director's clapper board](images/movie.jpg)

## Introduction

This project focuses on using data concerning recently successful movie titles. The goal is analysis helpful to the launch of a new studio.

## Objectives

This project explores the following questions and why:

* What are the recent top titles, by gross earnings?
* Which are the top performing studios? How fluid are their rankings
* What are the most frequently produced genres? ...The biggest earning?
* What is the genre mix for top studios?

# The Dataset

Project data resources were provided for this project in compressed (gunzip), flat files from Flatiron School's [Learn.co repository](https://github.com/learn-co-students/dsc-mod-1-project-v2-1-online-ds-ft-120919). Resources represent movie, studio, and budget-related data from the following sources:
* Box Office Mojo
* IMDB
* Rotten Tomatoes
* TheMovieDB.org

# Featured Notebooks/Analysis

Note: Some of the notebook and directory names may have been changed, since this project originally was developed (ergo, code refactoring may be required to duplicate project results).

* [`making-movies`: **Jupyter Notebook**](making-movies.ipynb): containing code written for this project and comments explaining it.

* [`movies-q1`](notebooks/movies-q1.ipynb): [notebook segment] _Top Grossing Titles_
    - Explore the highest gross recent movies
    - Visualize earnings distribution
    - Custom compute select earnings quantiles
    - View correlations: budget, gross, net, ROI


* [`movies-q2`](notebooks/movies-q2.ipynb): [notebook segment] _Top Grossing studios_
    - Explore top studios by gross earnings
    - Explore highest earnings by title
    - Slice dataframes and create a function to plot the top - 10 titles from each of the top studios


* [`movies-q3`](notebooks/movies-q3.ipynb): [notebook segment] _Genre and Studio Genre Mix_
    - Explore genre count and frequency
    - Join SQLite3 tables in Pandas: Plot earnings by genre in the most recent year and over the three most recent years, on a single figure
    - Visualize studio mix: movie count by genre for top - studios


* [`movies-data-conditioning`](notebooks/movies-data-conditioning.ipynb): [notebook segment] Loading the data
    - Load and inspect the 11 zipped data files as Pandas dataframes
    - Standardize naming conventions
    - Convert to SQLite3 database tables
    -  Validate conversion in Pandas.
    - Extract and expand genres
    - Drop tables


* [`movies-clean-transform`](notebooks/movies-clean-transform.ipynb): [notebook segment] Preparing data for analysis
    - View and convert datatypes
    - Update cleaned tables to Sqlite3

#### Box Office and the Bottom Line Analysis

Project results suggest a formula at work, in the movie business. The ratio of genres produced by top studios seems to have remained fairly constant. We can verify that by analyzing more closely central tendencies of top studios, including budget - spend and peak release cycles by genre.

Of course, there were a number of tables we did not yet explore. A more comprehensive reviews database could be valuable. Current resources do not indicate which reviews were provided prior to home release, or when income was generated, facts which make them less useful to predictive investigation but which may be resolved through feature engineering.

We do see a strong and rewarded showing by sequels, series, and fantasy (whether live - action, animated, or computer - generated). This is good news, for an industry that is currently increasing its footprint across platforms, from theaters and festivals to streaming services.

Adventure, action, comedy, and drama seem to be the ways to go. ROI consideration could be informative. It takes a lot of budget to make a blockbuster, but there do seem to be sweet spots where a relatively modest investment is more likely than not to result in a comfortable return.

For big swings, we need to determine how to deal with outliers. Many of the movies that made the most cost the most.


#### Visualizations & EDA

* visualizations, with corresponding interpretations are included within the `making-movies` and `q` ("question") notebook(s).

### Non-Technical Presentation

* [presentation.pdf](presentation.pdf) summarizing  methodology and findings


# Technologies
* Python
    - Pandas
    - Numpy
    - Matplotlib
    - Seaborn
* Sqlite3
* Jupyter Notebooks

```python

```
