# Python API Challenge

Challenge to pull city weather data for over 500 cities via API and populate charts to identify relationships between city location and temperature, humidity, cloudiness, and wind speed. 

Code may be reviewed in the [WeatherPy.ipynb](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/WeatherPy.ipynb) file.

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

![Temperature (F) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/lat_vs_temp.png?raw=true)

* Humidity (%) vs. Latitude

![Humidity (%) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/lat_vs_humidity.png?raw=true)

* Cloudiness (%) vs. Latitude

![Cloudiness (%) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/lat_vs_cloudiness.png?raw=true)

* Wind Speed (mph) vs. Latitude

![Wind Speed (mph) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/lat_vs_windspeed.png?raw=true)

Ran linear regression on each relationship (by Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude).

* Northern Hemisphere - Temperature (F) vs. Latitude

![Northern Hemisphere - Temperature (F) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/Northern%20Hemisphere%20Latitude%20vs%20Max%20Temperature%20(F).png?raw=true)

* Southern Hemisphere - Temperature (F) vs. Latitude

![Southern Hemisphere - Temperature (F) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/Southern%20Hemisphere%20Latitude%20vs%20Max%20Temperature%20(F).png?raw=true)

* Northern Hemisphere - Humidity (%) vs. Latitude

![Northern Hemisphere - Humidity (%) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/Northern%20Hemisphere%20Latitude%20vs%20Humidity%20(%25).png?raw=true)

* Southern Hemisphere - Humidity (%) vs. Latitude

![Southern Hemisphere - Humidity (%) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/Southern%20Hemisphere%20Latitude%20vs%20Humidity%20(%25).png?raw=true)

* Northern Hemisphere - Cloudiness (%) vs. Latitude

![Northern Hemisphere - Cloudiness (%) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/Northern%20Hemisphere%20Latitude%20vs%20Cloudiness%20(%25).png?raw=true)

* Southern Hemisphere - Cloudiness (%) vs. Latitude

![Southern Hemisphere - Cloudiness (%) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/Southern%20Hemisphere%20Latitude%20vs%20%20Cloudiness%20(%25).png?raw=true)

* Northern Hemisphere - Wind Speed (mph) vs. Latitude

![Northern Hemisphere - Wind Speed (mph) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/Northern%20Hemisphere%20Latitude%20vs%20Wind%20Speed%20(mph).png?raw=true)

* Southern Hemisphere - Wind Speed (mph) vs. Latitude

![Southern Hemisphere - Wind Speed (mph) vs. Latitude](https://github.com/szerpa17/API-Challenge/blob/master/WeatherPy/images/Southern%20Hemisphere%20Latitude%20vs%20Wind%20Speed%20(mph).png?raw=true)


### Observations
* The northern and southern hemispheres have an almost inverse relationship (due to the scale of each) with max temperature. Though the northern hemisphere has a negative linear relationship and the southern hemisphere has a positive linear relationship. Both charts both demonstrate that cities that are closer to the equator experience higher max temperatures. 
* Based on the regression line, no clear correlation was found for humidity, cloudiness, and wind speed when these values were compared with latitude. This can allow us to infer that temperature is not the only cause or explanation for differences in these weather conditions among cities (the environment, distance from bodies of water, and elevation may instead be considered as factors). 
* The Pearson R value somewhat supported the linear regression functions for temperature and elevation as it demonstrated that the function explained 41 percent of the northern hemisphere and 51 percent of southern hemisphere data. The Pearson R values for the other regressions also support the lack of correlation as the numbers were near zero.
