# Python API Challenge

Challenge to pull city weather data for over 500 cities via API and populate charts to identify relationships between city location and temperature, humidity, cloudiness, and wind speed. 

![Equator](Images/equatorsign.png)

## Tools 
* Google Places API
* Python
* Python Packages:
    * pandas
    * matplotlib.pyplot
    * numpy
    * requests
    * time
    * json
    * linregress


## WeatherPy

This file was used to create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. 

Created a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Ran linear regression on each relationship (by Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude).

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude
