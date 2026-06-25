# Fuel Efficiency & the 1973 Oil Crisis — Exploratory Data Analysis

## Overview
In this analysis I explore the impact of the 1973 oil crisis, and its aftermath by finding the most significant factors influencing the fuel efficiency of the car, based on the MPG (Miles Per Gallon) dataset provided by Seaborn library. The dataset contains data from years 1970 to 1982 regarding 398 models produced in three different parts of the world: USA, Europe and Japan. Based on that I will determine which geographical region was most affected, and why.

## Key Findings
- USA improved fuel efficiency by 29.7% after the crisis — the largest improvement of any region
- The strongest predictor of fuel efficiency is vehicle weight (correlation: -0.83 with MPG)
- American cars were significantly heavier than European and Japanese counterparts, giving them the most room to improve
- Despite the biggest improvement, USA remained behind Japan (30.8 MPG) and Europe (28.2 MPG) post-crisis
- Possible sampling bias caveat: the dataset contains far more US models than EU/Japan, which may affect regional comparisons

## Methodology
1. Data cleaning — handled null values in `horsepower` column (~1.8% of data, dropped safely)
2. Correlation analysis — identified key factors influencing MPG
3. Time series visualisation — tracked MPG, weight, displacement, and cylinders by region over time
4. Pre/post crisis comparison — quantified percentage improvement per region (1970–73 vs 1974–80)
5. Limitations assessment — flagged potential sampling bias in regional representation

## Tools & Libraries
- Python (pandas, numpy, matplotlib, seaborn)
- Dataset: [Seaborn MPG dataset](https://github.com/mwaskom/seaborn-data/blob/master/mpg.csv)
