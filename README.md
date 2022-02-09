# Surfs_Up

## Overview of the Analysis
The purpose of this analysis was to determine whether or not a Surf Shop in Oahu that served ice-cream would be successful year round. In order to determine this, an analysis of the temperatures would be completed to determine if the weather was warm enough for surfing and ice-cream year round, making for a successful business. 

The analysis was completed using a few tools. First, the data was gathered from a SQLite database. Which offered an easier to access database that was saved locally to my computer. Additionally, the analysis was written in Python using Jupyter Notebooks. In order to connect our Python Files to this SQLite database, SQLalchemy was used. SQLalchemy is an installable package for python files that establishes a connection to a local SQL database. Once all of these tools were properly installed and connected, the analysis could begin. 

## Results
A few queries were written in order to grab the neccessary data from the SQL database. There were 2 tables within the database. First, a table for the different Weather Stations that recorded data for Oahu. In total there were 9, each with a unique station id and geographic location (latitude and longitude). The other table consists of weather measurements everyday, recording the percipitation and temperature from each station. The data dates from the beginning of 2010 to around August of 2017. 

The first task was to determine the weather statistics from the month of July. Rather than selecting one specific year, a query was run to select all the weather data from all days in June across all the years in the database. Once the query was preformed, summary statistics were determined and are shown below. 

![alt text](https://raw.githubusercontent.com/KitWilliams07/Surfs_Up/main/june.png)

## Summary 

