# python-api-challenge
## Part 1 - WeatherPy
### Overview
 A Python script that visualizes the weather of 500+ cities across the world of varying distance from the equator. A representative model of weather across world cities were created by using: 
* [simple Python library](https://pypi.python.org/pypi/citipy), and the
* [OpenWeatherMap API](https://openweathermap.org/api)

### Analysis
#### Scatter plots
Scatter plots will showcase the following relationships:
* Temperature (F) vs. Latitude
![Alt text](/WeatherPy/Images/City Latitude vs Max Temperature.png?raw=true "Figure 1")

* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

#### Linear regression
Linear regressions were run on separate plots in the Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):
* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

## Part II - VacationPy
Weather data will be used to plan future vacations. The following were created by using:
* jupyter-gmaps, and the 
* Google Places API

### Analysis
#### Humidity Heat Map
A heat map that displays the humidity for every city from Part I - WeatherPy.

#### Find hotel for each city with ideal weather conditions.
The DataFrame was narrowed to find the ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

  * Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.

  * **Note:** Feel free to adjust to your specifications but be sure to limit the number of rows returned by your API requests to a reasonable number.

Google Places API was used to find the first hotel for each city located within 5000 meters of coordinates.

#### Updated Humidity Heat Map
Humidity heatmaps now have the hotels plotted with the following information: 
* Hotel Name, 
* City, 
* Country.
