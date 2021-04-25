# python-api-challenge
Python assignment covering Python requests, APIs, JSON traversals, and data visualization (Due: 04-14-2021)

--------------------

# Instructions

## Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter..."_

But, if pressed, how would you **prove** it?


## Part I - WeatherPy

In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

### Final Plots
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/lat_vs_max_temp.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/lat_vs_humidity.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/lat_vs_cloudiness.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/lat_vs_wind.png)

The second requirement is to run linear regression on each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

### Final Plots

![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/northern_lat_vs_maxtemp_regress.png) ![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/southern_lat_vs_maxtemp_regress.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/northern_lat_vs_humidity_regress.png) ![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/southern_lat_vs_humidity_regress.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/lat_vs_humidity_regress_equator.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/northern_lat_vs_cloudiness_regress.png) ![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/southern_lat_vs_cloudiness_regress.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/northern_lat_vs_wind_regress.png) ![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/WeatherPy/images/southern_lat_vs_wind_regress.png)

## Part II - VacationPy

Now let's use your skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.


To complete this part of the assignment, you will need to do the following:

* Create a heat map that displays the humidity for every city from Part I.

* Narrow down the DataFrame to find your ideal weather condition.

* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

### Final Plots
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/VacationPy/images/initial_heat_layer.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/VacationPy/images/marker_layer.png)
![](https://github.com/moriahtaylor1/python-api-challenge/tree/main/VacationPy/images/marker_info.png)



-------------------------
### Instructions Copyright

Trilogy Education Services © 2020. All Rights Reserved.
