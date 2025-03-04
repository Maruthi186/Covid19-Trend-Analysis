# Covid19 Trend Analysis

Covid-19 impacted the world significantly, and analyzing trends in case numbers helps us understand the spread and severity of the virus. This project provides an in-depth analysis of Covid-19 case trends using Python, Pandas, NumPy, Matplotlib, and Scikit-learn.

## Overview
This project:
- Cleans and preprocesses Covid-19 case data.
- Analyzes confirmed, recovered, and death cases.
- Groups data by country and date.
- Visualizes trends using line plots.
- Implements basic machine learning techniques for missing value imputation.

## Features
- Data Preprocessing: Reads raw CSV data, removes unnecessary columns, renames headers, and converts date formats.
- Handling Missing Data: Uses Scikit-learn’s SimpleImputer to fill missing values.
- Grouping and Aggregation: Groups data by country and date to observe trends.
- Data Analysis: Computes mean, max, min, standard deviation, and other statistics.
- Visualization: Generates line plots to visualize the Covid-19 case trends.
- Time-Series Smoothing: Applies a rolling window (moving average) to smooth out fluctuations.

## Dataset

The project utilizes a dataset named covid_19_data.csv, which consists of the following columns:

| Column Name      | Description                                   |
|-----------------|----------------------------------------------|
| SNo            | Serial number (removed during processing)   |
| ObservationDate | Date when data was recorded               |
| Province/State | State/Province (some values are null)      |
| Country/Region | Country name                                |
| Last Update   | Timestamp of last update (removed)         |
| Confirmed     | Total confirmed cases                       |
| Deaths        | Total death cases                           |
| Recovered     | Total recovered cases                       |

After preprocessing, the dataset is cleaned and transformed into:

| Date       | State       | Country      | Confirmed | Deaths | Recovered |
|------------|------------|-------------|-----------|--------|-----------|
| 2020-01-22 | Anhui      | China       | 1         | 0      | 0         |
| 2020-01-22 | Beijing    | China       | 14        | 0      | 0         |
| 2020-01-22 | Hubei      | China       | 444       | 17     | 28        |

## Libraries Used 
- Pandas (Data processing and analysis)  
- NumPy (Numerical operations)  
- Matplotlib (Data visualization)  
- Scikit-learn (Handling missing data)  
