# World_Weather_Analysis

## Overview
 Weather conditions are one of the major factors when considering taking a trip. Vacationers check the weather frequently in advance of their trip hoping for an optimal experience. This project has been undertaken to collect, analyze and visualize weather data for cities across the globe and provide would be travelers with information that will allow them to determine their ideal travel destination based on weather conditions.

### Resources used to Complete the Analysis
* **CSV Files:** 
[Weather_Database.csv](hhttps://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/Weather_Database/WeatherPy_Database.csv, 
[WeatherPy_vacation.csv]( https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/Vacation_Search/WeatherPy_vacation.csv)
* **Jupyter Notebook Files:**: 
[Weather_Database.ipynb](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/Weather_Database/Weather_Database.ipynb), 
[Vacation_Search.ipynb](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/Vacation_Search/Vacation_Search.ipynb),
[Vacation_Itinerary.ipynb]( https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/Vacation_Itinerary/Vacation_Itinerary.ipynb)

* **Python**: Python v3.7.11, Dependencies: Pandas, Matplotlib, CitiPy, SciPy, Python Requests, APIs, JSON Traversals

## Weather Database
Generated a random set of around latitudes and longitudes and made an API call on current weather for the nearest corresponding cities. 

Retrieved the following data from the API call: 
* Latitude and longitude
* Maximum temperature
* Percent humidity
* Percent cloudiness
* Wind speed
* Current Weather description 

## Vacation Search
Based on a prospective vacationer's weather preferences, the are able to identify potential travel destinations and nearby hotels. The map displays destinations using pop-up markers on a marker layer-map.

### Sample Travel Destinations

![WeatherPy_vacation_map](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/Vacation_Search/WeatherPy_vacation_map.png)

## Vacation Itinerary 
Using the Google Directions API, a demo itinerary was put together that shows the route between four cities in the United States of America.

![WeatherPy_travel_map](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/Vacation_Itinerary/Weather_Py_Travel_Map.png)

## Statistical Analysis
Data for global cities was plotted, and then linear regression was utilized to find the relationship between the following variables: 

* Latitude and Maximum Temperature
* Latitude and Humidity
* Latitude and Cloudiness
* Latitude and Wind Speed

### Scatter Plots 
Scatter plots were generated for each weather parameter based on  the latitude for all cities to show how weather parameters change based on latitude. 

![City Latitude vs. Max Temperature](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LatVsMT.png)
![City Latitude vs. Max Humidity](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LatVsHum.png)
![City Latitude vs. Cloudiness](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LatVsCloud.png)
![ City Latitude vs. Wind Speed](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LatVsWS.png)

### Linear Regression on the Northern and Southern Hemispheres
Applied linear regression to the Northern and Southern Hemispheres, on the following weather parameters: maximum temperature, humidity, cloudiness, and wind speed.

#### Maximum Temperature
![Linear Regression on the Northern Hemisphere for Maximum Temperature](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LinRegNorHemMT.png)
![Linear Regression on the Southern Hemisphere for Maximum Temperature](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LinRegSouHemMT.png)

#### Percent Humidity
![Linear Regression on the Northern Hemisphere for Percent Humidity](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LinRegNorHemH.png)
![Linear Regression on the Southern Hemisphere for Percent Humdity](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LinRegSouHemH.png)

#### Percent Cloudiness
![Linear Regression on the Northern Hemisphere for Percent Cloudiness](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LinRegNorHemC.png)
![Linear Regression on the Southern Hemisphere for Percent Cloudiness](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LinRegSouHemC.png)

#### Wind Speed
![ Linear Regression on the Northern Hemisphere for Wind Speed](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LinRegNorHemWS.png)
![ Linear Regression on the Southern Hemisphere for Wind Speed](https://github.com/dannybarto/World_Weather_Analysis/blob/3c297920a5aa95a7f5ec2b899aa0fa38b1d8ed86/weather_data/LinRegSouHemWS.png)
