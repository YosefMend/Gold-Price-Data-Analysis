# Gold-Price-Data-Analysis
This project analyzes the historical prices of gold from 2000 to 2023, examines the relationship between gold prices and the strength of the US Dollar (USD) Index, and uses historical data to identify best buy-in and sell points.


## Table of Contents
- [Introduction](#introduction)
- [Data Sources](#data-sources)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modeling and Forecasting](#modeling-and-forecasting)
- [Results](#results)
- [Conclusion](#conclusion)
- [How to Use](#how-to-use)
- [Requirements](#requirements)


## Introduction
The aim of this project is to perform a comprehensive analysis of gold prices, identify seasonal trends and understand the correlation between gold prices and the USD Index.

## Data Sources
- **Gold Prices**: Historical gold prices sourced from [yahoo finance](https://finance.yahoo.com/quote/GC%3DF/history/).
- **USD Index**: Historical USD Index values sourced from [yahoo finance]((https://finance.yahoo.com/quote/DX-Y.NYB/history/)).

## Data Preprocessing
The data preprocessing involved:
- Using yfinance API to load data sets.
- Converting date columns to datetime format.
- Handling missing values with forward filling.
- Aggregating data by month and year.
- Calculating moving averages (50-day, 100-day, 200-day).
- Normalizing data for comparison.
- Grouping Tables

All preprocessing steps are documented in the [datapreprocessing.ipynb](notebooks/datapreprocessing.ipynb) notebook.

## Exploratory Data Analysis
We performed a detailed EDA to uncover insights such as:
- Monthly and yearly average prices.
- Yearly percent changes.
- Seasonal trends in gold prices.
- Correlation with the USD Index.
- Potential best buy and sell times.

(The EDA notebook contains detailed plots and analysis)

See the [ExploratoryDataAnalysis.ipynb](notebooks/ExploratoryDataAnalysis.ipynb) notebook for details.

## Results
My analysis showed:
- Seasonal patterns in gold prices, with [specific months] having higher prices.
- Seasonal patterns in gold prices, with [specific months] having lower prices.
- Which months are more probably to show an above 4.5% increase of price month to month.
- A negative correlation between gold prices and the USD Index.

The detailed results and visualizations can be found in the notebooks.

## Conclusion
The analysis provided insights into the seasonal trends and the dependency of gold prices on the USD Index.

Future work could include expanding the dataset to incorporate other economic indicators and creating forecasting models to predict price fluctuations and project better buy-in times.

## Requirements
The project requires the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- prophet
- scikit-learn
