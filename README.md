# World Weather Analysis By Alec Ngai

## Overview

This analysis looks at different weather patterns around the global and offers insights to travelers who want to book a trip. There are three folders here that offer different levels of analysis: weather database, vacation search, and vacation itinerary.

### Weather Database

This folder uses Open Weather Map API to pull weather information on over 722 different cities around the world into a Dataframe which we convert and save as csv. The csv consists of the following data: 

1. City 
2. Country
3. Latitude
4. Longlitude
5. Max Temperature
6. Humidity
7. Cloudiness
8. Wind Speed
9. Current Weather Description

This CSV will be the foundation of our analysis to allow us to provide a travel planning service to clients. 

### Vacation Search

This folder takes the information gained in the weather database and uses Google Maps API to plot different travel destinations with a hotel at each location. For example, the image below shows the locations of all the places in the database that have an daily maximum temperature between 20 and 25 degrees celcius.

![vacation_search_map](https://github.com/alecngai/06_World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### Vacation Itinerary

This folder takes the search information from the search folder and uses Google Maps directions API to create a vacation itinerary. For example, the image below shows a 4 stop itinerary in Northern California that features Ukiah, Carson City, Laguna, and Half Moon Bay.

![vacation_itinerary_map](https://github.com/alecngai/06_World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

Also, as with the vacation search folder, there is a hotel at each location.

![vacation_itinerary_markers](https://github.com/alecngai/06_World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
