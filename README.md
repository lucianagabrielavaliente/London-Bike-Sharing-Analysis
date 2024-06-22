# London Bike Sharing Analysis

This repository contains a project that analyzes the London Bike Sharing Dataset from Kaggle. The analysis involves data exploration and visualization, with the final visualizations created using Tableau.

## Table of Contents

1. [Dataset](#dataset)
2. [Project Structure](#project-structure)
3. [Data Exploration](#data-exploration)
4. [Visualizations](#visualizations)

## Dataset
The dataset is sourced from three different platforms:
1. [Transport for London (TfL) Open Data](https://cycling.data.tfl.gov.uk/)
2. [Freemeteo.com](https://freemeteo.com) - for weather data
3. [UK Government Bank Holidays](https://www.gov.uk/bank-holidays)

The result is the folowwing dateset in Kaggle:
 [Kaggle - Final Dataset](https://www.kaggle.com/datasets/hmavrodiev/london-bike-sharing-dataset)

The dataset covers the period from January 1, 2015, to December 31, 2016, and includes the following fields:
- `timestamp`: Timestamp for grouping the data
- `cnt`: Count of new bike shares
- `t1`: Real temperature in Celsius
- `t2`: Feels-like temperature in Celsius
- `hum`: Humidity in percentage
- `wind_speed`: Wind speed in km/h
- `weather_code`: Category of the weather
- `is_holiday`: Boolean field indicating if the day is a holiday
- `is_weekend`: Boolean field indicating if the day is a weekend
- `season`: Meteorological season (0=spring, 1=summer, 2=fall, 3=winter)

### Weather Code Descriptions
- `1`: Clear
- `2`: Scattered clouds
- `3`: Broken clouds
- `4`: Cloudy
- `7`: Rain / Light Rain shower / Light rain
- `10`: Rain with thunderstorm
- `26`: Snowfall
- `94`: Freezing Fog

## Project Structure

The repository contains the following files:
- `london_merged.csv`: The original dataset
- `london-bike-sharing-eda.ipynb`: Jupyter notebook for data exploration and analysis
- `london_bikes_final.xlsx`: Final cleaned dataset used for Tableau visualizations

## Data Exploration

The data exploration process is performed in the Jupyter notebook `london-bike-sharing-eda.ipynb`. Key steps include:
- Downloading the dataset using Kaggle API
- Checking for null values and unique counts in columns
- Renaming columns for clarity
- Converting humidity values to percentage
- Mapping numerical values to categorical descriptions for seasons and weather

  ## Visualizations

The final cleaned dataset is used to create various visualizations in Tableau, including:
- Moving average visualization
- Total rides visualization
- Temperature vs. wind speed heatmap
- Weather and hour bar charts

### Tableau Dashboard

You can view the Tableau dashboard [here](https://public.tableau.com/app/profile/luciana.valiente/viz/london-bike-rides/Dashboard1?publish=yes)).

![Tableau Dashboard Screenshot](https://github.com/lucianagabrielavaliente/London-Bike-Sharing-Analysis/assets/54379062/2ddb8d34-b4bd-4381-8a57-e3fc7e476422)
![Tableau Dashboard Screenshot](https://github.com/lucianagabrielavaliente/London-Bike-Sharing-Analysis/assets/54379062/c3e17f6d-2f00-4836-bc87-cfded6be35b0)

