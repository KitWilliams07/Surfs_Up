# Surfs_Up

## Overview of the Analysis
The purpose of this analysis was to determine whether or not a Surf Shop in Oahu that served ice-cream would be successful year round. In order to determine this, an analysis of the temperatures would be completed to determine if the weather was warm enough for surfing and ice-cream year round, making for a successful business. 

The analysis was completed using a few tools. First, the data was gathered from a SQLite database. Which offered an easier to access database that was saved locally to my computer. Additionally, the analysis was written in Python using Jupyter Notebooks. In order to connect our Python Files to this SQLite database, SQLalchemy was used. SQLalchemy is an installable package for python files that establishes a connection to a local SQL database. Once all of these tools were properly installed and connected, the analysis could begin. 

## Results
A few queries were written in order to grab the neccessary data from the SQL database. There were 2 tables within the database. First, a table for the different Weather Stations that recorded data for Oahu. In total there were 9, each with a unique station id and geographic location (latitude and longitude). The other table consists of weather measurements everyday, recording the percipitation and temperature from each station. The data dates from the beginning of 2010 to around August of 2017. 

The first task was to determine the weather statistics from the month of July. Rather than selecting one specific year, a query was run to select all the weather data from all days in June across all the years in the database. Once the query was preformed, summary statistics were determined and are shown below. 

![alt text](https://raw.githubusercontent.com/KitWilliams07/Surfs_Up/main/june.png)


This same process was repeated for the month of December. The summary statistics for December are shown below. 

![alt text](https://raw.githubusercontent.com/KitWilliams07/Surfs_Up/main/december.png)


After looking at these summary statistics for these months, a few key observations can be drawn. 

First, the average temperature for June across the 7 years is 75 degrees while the average for December was 71 degrees. Additionally, the maximum recorded temperature in June was 85 degrees and in December it was 83 degrees. Lastly, the minimum temperature for June was 64 degrees while for December it was 56 degrees. It is important to note that each month had a comaparable number of data points, both months falling between 1500-1700 recorded days. 

## Summary 
From hese observations a few conclusions can be drawn. The first being that if we are only basing the success on the business based on temperature recordings, then the business should thrive year round because the temperature differences between June and December for all of these years is negligible. I personally cannot feel the difference between the average temperatures of 75 and 71 degrees and the maximum temperatures of 85 and 83 degrees.

However, I would suggest a more detailed analysis before recommending that this business would be a sound idea. Using the data we are given, a logical next step to provide a more detailed analysis would be to gather some numbers on the amount of precipitation each month recieves. Most people do not enjoy surfing and eating ice-cream if it is pouring rain. I think that having some idea of which months are the rainest would make important business deicisons. 

In addition, another query that could be run would be to only select data from the Weather station that is the closest. This data was compiled using data from all 9 weather stations. However every side of the island may experience different levels of sunlight, rain, wind, etc. As a result I believe that selecting the Weather Station that is the closest to the desired location of the Surf Shop would give more accurate readings of the weather of that exact part of the island. While I do not suspect there will be a major difference I see no value in including weather data from all 9 stations when the weather right next to the shop would be the most accurate. 
