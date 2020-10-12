# Part I WeatherPy
In this example, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I use a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

*Note: all the output images for this part can be found in the folder **output_data**.*

First, I use scatterplot demonstrating the relationship and trend between City Latitude and a series of other variables:
* Tempurature vs. Latitude

* Humidity vs. Latitude

* Cloudiness vs. Latitude


The second task is to deetect relationships between variables, with northern hemisphere and southrn hemisphere analyzed separately. 
Below are some examples of the output correlations:
* Northern Hemisphere - Temperature (F) vs. Latitude

* Southern Hemisphere - Temperature (F) vs. Latitude

* Northern Hemisphere - Humidity (%) vs. Latitude

* Southern Hemisphere - Humidity (%) vs. Latitude


# Part II VacationPy
In this part I use weather data to plan future vacations. Jupyter-gmaps and the Google Places API fare also used for this part.
*Note: all the output images for this part can be found in the folder **Images**.*

Here are the main tasks demonstrated:
* Create a heat map that displays the humidity for every city from the part I of the homework.

* Narrow down the DataFrame to find your ideal weather condition. For example:
  * A max temperature lower than 280 degrees but higher than 260.
  * Wind speed less than 10 mph.
  * Zero cloudiness.

* Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.
* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.
* Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
