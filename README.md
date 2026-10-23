# Airbnb Listings: Price Drivers and K-means Clustering
## Overview
This project analyses a dataset of 279,712 Airbnb listings across several major cities to understand the main drivers of listing prices and how prices relate to location. It was completed as a group project for the Coding course at Bocconi University.

## Objectives
1. Explore the dataset to identify the most important variables and general trends.
2. Analyse which factors are most related to listing prices.
3. Implement the K-means clustering algorithm from scratch and apply it to identify areas with similar price levels in New York City.

## Methods
* Data cleaning: selection of relevant variables, removal of rows missing essential values (location, price), median imputation for other numerical variables
* Exploratory analysis: distributions, host characteristics, price by room type, scatter plots and correlation matrices
* Outlier analysis: comparison of results with and without extreme prices (beyond 3 standard deviations)
* K-means clustering implemented from scratch in NumPy (centroid initialisation, squared Euclidean distances, assignment and update steps, convergence criterion), validated on a simulated 2D dataset, then applied to New York listings using latitude, longitude and price

## Key findings
* Prices are strongly right skewed: most listings are affordable, while a small number are extremely expensive.
* Accommodation size (number of guests and bedrooms) is the variable most related to price; review scores and minimum stay show almost no relationship.
* This relationship becomes much clearer once extreme prices are removed, showing how outliers can hide underlying patterns.
* K-means identifies three geographically coherent price zones in New York, with a high-price cluster in central Manhattan (average around $208 per night) against around $79 to $91 in the other two areas.
* Keeping price outliers produces more contrasted clusters, suggesting that extreme prices carry real economic information rather than pure noise: a trade-off between robustness and signal.

## Tools
Python, NumPy, pandas, Matplotlib, Jupyter Notebook

## Data
The analysis uses a publicly available Airbnb listings dataset (Listings.csv, 279,712 listings, 33 variables). The dataset is not included in this repository.

## Authors
Group project for the Coding course at Bocconi University.
