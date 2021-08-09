# World Weather Analysis By Alec Ngai

## Overview

This analysis looks at different weather patterns around the global. We use input statements to filter the data for the of the traveller weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, you will create a travel route between the four cities as well as a marker layer map.

## Resources
Data source: WeatherPy_Database.csv, WeatherPy_vacation.csv
Software: Python 3.9.4, Visual Studio Code, 1.58.1, conda 4.10.1
API: OpenWeatherMap, Places, Geocoding, Maps Javascript, Directions
 
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
