# Olympics 1952-2014, looking at some world trends

*Author: Ximena Leyva Peralta*\
*"Analyze Data with Python" Codecademy course, final project*\
*August 20th, 2024*

## Introduction

This project explores and visualizes global trends in Olympic performance, highlighting how a country's or continent's origin influences results.\
\
My goal is to practice dataset handling, data cleaning, visualization, and statistical hypothesis testing without delving into explanations for the observed trends.

## Dataset
The final dataset is provided in `dataset/directory.csv`.\
\
Quick summary of the columns:
- **Country**: Country name
- **Code**: 3-letter code for country
- **Population**: Latest estimate of country's population
- **GDP per Capita**: Latest estimate of country's GDP per capita (USD)
- **Total medals**: Total medals won between 1952-2014 across all events
- **Continent**: Code for country's continent (see `continent_names` below for conversion table)
- **Total gold**: Total gold medals won between 1952-2014 across all events
- **Total silver**: Total silver medals won between 1952-2014 across all events
- **Total bronze**: Total bronze medals won between 1952-2014 across all events
- **Medals per capita**: Calculated as Total medals/Population
- **Total medal val**: Total value of country's medals calculated by assigning gold=3, silver=2, bronze=1
- **Avg medal val**: Calculated as Total medal val/Total medals\
\
Initial dataset is from [this Kaggle entry](https://www.kaggle.com/datasets/the-guardian/olympic-games), which credits the IOC Research and Reference Service and The Guardian's Datablog. 

## Project Goals

* **Explore Trends in Olympic Performance Worldwide:** Analyze the distribution of Olympic medals across different countries and continents to identify patterns and trends.

* **Visualize Performance Across Countries and Continents:** Create clear and insightful visualizations to compare the Olympic performance of various continents.

* **Perform Statistical Hypothesis Tests:** Formulate and test hypotheses based on the observed data. This includes performing various statistical tests to validate or challenge these hypotheses.

## Methodology
* **Data Preparation:** Results from summer and winter olympics were combined. Countries with no GDP per capita or population data and with zero medals were deleted.

* **Visualization:** Seven figures were created using Matplotlib. They can be found in png format in the `./figures` directory.

* **Statistical Tests:** Hypotheses were formulated based on observed trends, such as the relationship between a country’s GDP per capita and its Olympic medal count. Statistical tests, including t-tests and ANOVA, were conducted to validate these hypotheses using Python's SciPy and Statsmodels libraries.

## Results
* **Trends Identified:** The analysis revealed that wealthier and less populated countries tend to win more medals, but there are notable exceptions. Additionally, some continents consistently outperform others, with Europe and North America leading in overall medal counts.

* **Statistical Findings:** Some hypotheses supported by statistical tests are: GDP per capita is positively correlated with Olympic success, a country's continent influences its likelihood of winning a gold medal, and European countries have won, on average, more medals than the global average.

## Future Work
Future work could involve a deeper exploration of the underlying factors influencing Olympic success, such as cultural, historical, and political factors. Additionally, incorporating more recent data and expanding the analysis to include Winter Olympics could provide a more comprehensive view of global Olympic performance.