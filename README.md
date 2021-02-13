# Python-Api-Challenge
## General Description
This repository includes two projects: "WeatherPy" and "VacationPy". The first one analyzes the weather information of 500 random cities across the world. As for the second project, it uses the list of 500 cities from the WeatherPy project and narrows it based on my weather preferences for my ideal vacation spot. Additionally, it locates the cities in the map and shows one hotel option for each city.
## Objectives
### WeatherPy
Based on a randomly generated list of 500 cities, this program aims to identify any possible correlation between the latitude and some of the weather conditions of each city: maximum temperature, humidity, cloudiness and wind speed.

The project is divided in 2 parts:
- The first part includes 4 scatter plots with the following information:
  - Temperature vs Latitude
  - Humidity vs Latitude
  - Cloudiness vs Latitude
  - Wind Speed vs Latitude
 - The second part divides the cities based on their latitude: Northern Hemisphere cities and Southern Hemisphere cities, and plots the same information as before. Additionally it runs a linerar regression on each relationship. 
  - Northern Hemisphere: Temperature vs Latitude
  - Southern Hemisphere: Temperature vs Latitude
  - Northern Hemisphere: Humidity vs Latitude
  - Southern Hemisphere: Humidity vs Latitude
  - Northern Hemisphere: Cloudiness vs Latitude
  - Southern Hemisphere: Cloudiness vs Latitude
  - Northern Hemisphere: Wind Speed vs Latitude
  - Southern Hemisphere: Wind Speed vs Latitude
  
  ### Results
  - There is a strong correlation between the the Northern Hemisphere cities (-.88)  and the max temperature. The higher the latitude, the lower the temperature.
  - However, we cannot say the same for the Southern Hemisphere cities where the correlation is .48.
  - As for the other weather conditions: Humidity, Cloudiness and Wind Speed, their values does not seem to vary based on the latitude of the cities. Their correlations are not strong.
  
  ## VacationPy
  Based on the list of cities generated in the WeatherPy project, a heatmap is created based on the himidity of each city. Additionally, a filtered city list is generated based on my weather preferences for my ideal vacation spot. Using the Google Places API, the program searches for a hotel within a 5000 meters radius of each of the cities coordinates (filtered list) and plots this information on top of the humidity heatmap.  
### Results

![alt text](https://github.com/PilarM0ntes/python-api-challenge/blob/main/Images/heatmap.png)
