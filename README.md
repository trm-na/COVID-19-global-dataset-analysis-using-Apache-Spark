# Analysis of the COVID-19 global dataset using Apache Spark

This repository includes the code to analyse a dataset with the number of confirmed cases of COVID-19 infections segregated by countries from January 22nd 2020 until March 9th 2023 using Apache Spark.

The dataset was retrieved from the [Centre for Systems Science and Engineering at Johns Hopkins University's GitHub](https://github.com/CSSEGISandData/COVID-19/blob/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_global.csv) for this study.

Additionally, a dataset to list the different countries and regions as well as the continents, extracted from the Country or Area and Continent columns from the [List of Countries by Continent by Statistics Times](https://statisticstimes.com/geography/countries-by-continents.php), with some slight modifications to fit the metadata in the COVID-19 dataset, is used.

Specifically, for each country, the mean number of daily confirmed cases for each month in the dataset is computed, for each continent, the mean, standard deviation, minimum and maximum of the daily confirmed cases for each week, considering only the 100 most affected states by the pandemic according to the trendline coefficient are computed, and finally, for each month, the 50 most affected states monthly according to the trendline coefficient are segregated into 4 groups using the clustering algorithm K-means.

## General pipeline

The code's general pipeline is depicted in the following image:

<img width="897" height="412" alt="image" src="https://github.com/user-attachments/assets/e45e5953-b062-4252-8c94-2b5fe6c5ae7d" />

## Data Transformation pipeline

The data transformation pipeline is depicted in the following image:

<img width="1176" height="457" alt="image" src="https://github.com/user-attachments/assets/6e683f0b-36ac-4962-b2c3-45a2f690ec7d" />


## Query 1 pipeline

The pipeline for query 1 is depicted in the following image:

<img width="885" height="210" alt="image" src="https://github.com/user-attachments/assets/77808437-5a8c-43ff-a98f-5d1053e29792" />


## Query 2 pipeline

The pipeline for query 2 is depicted in the following image:

<img width="1170" height="457" alt="image" src="https://github.com/user-attachments/assets/1207cbf4-57c0-4ab1-8c17-0e60535fca5e" />

## Query 3 pipeline

The pipeline for query 3 is depicted in the following image:

<img width="1184" height="509" alt="image" src="https://github.com/user-attachments/assets/7afe4d27-479c-4097-abf3-f4412060308d" />

<hr>
<br>This code is my submission for Cranfield University's Machine Learning and Big Data module assignment for the MSc in Computational and Software Techniques in Engineering - Computational Intelligence for Data Analytics.
