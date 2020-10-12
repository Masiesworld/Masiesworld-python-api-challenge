# Part I WeatherPy
In this example, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I use a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

*Note: all the output images for this part can be found in the folder **output_data**.*

First, I use scatterplot demonstrating the relationship and trend between City Latitude and a series of other variables:
* Tempurature vs. Latitude
![lat temp](https://user-images.githubusercontent.com/50465138/95777390-190e6900-0c94-11eb-953c-eddd982fc78e.png)

* Humidity vs. Latitude
![lat humidity](https://user-images.githubusercontent.com/50465138/95777407-21ff3a80-0c94-11eb-9c26-735c3e33763e.png)

* Cloudiness vs. Latitude
![lat clouds](https://user-images.githubusercontent.com/50465138/95777422-29bedf00-0c94-11eb-8389-f712e1d6c064.png)

The second task is to deetect relationships between variables, with northern hemisphere and southrn hemisphere analyzed separately. 
Below are some examples of the output correlations:
* Northern Hemisphere - Temperature (F) vs. Latitude
![Fig1](https://user-images.githubusercontent.com/50465138/95777516-5246d900-0c94-11eb-8087-d894049b1a5f.png)

* Southern Hemisphere - Temperature (F) vs. Latitude
![Fig2](https://user-images.githubusercontent.com/50465138/95777519-54a93300-0c94-11eb-9853-188f054091e5.png)

* Northern Hemisphere - Humidity (%) vs. Latitude
![Fig3](https://user-images.githubusercontent.com/50465138/95777543-64c11280-0c94-11eb-973c-6112cd62342c.png)

* Southern Hemisphere - Humidity (%) vs. Latitude
![Fig4](https://user-images.githubusercontent.com/50465138/95777544-64c11280-0c94-11eb-9be3-2dbd870b6489.png)


## Three major findings:
1. There is a strong correlation between max tempurature and latitude;
2. There tends to be minimal relationship between humidity and latitude in South hemisphere. (r<0.1)
3. There is weak correlation between Cloudiness (%) and latitude.


# Part II VacationPy
In this part I use weather data to plan future vacations. Jupyter-gmaps and the Google Places API fare also used for this part.

*Note: all the output images for this part can be found in the folder **Images**.*

Here are the main tasks demonstrated:
* Create a heat map that displays the humidity for every city from the part I of the homework.
![Heatmap](https://user-images.githubusercontent.com/50465138/95775198-f7ab7e00-0c8f-11eb-8d8f-1bac0bf6a3f3.png)

* Narrow down the DataFrame to find your ideal weather condition. For example:
  * A max temperature lower than 280 degrees but higher than 260.
  * Wind speed less than 10 mph.
  * Zero cloudiness.

* Drop any rows that don't contain all three conditions. 
* Using Google Places API to find the first hotel for each city located within 5000 meters of the coordinates.
* Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
![hotelmap](https://user-images.githubusercontent.com/50465138/95775204-f8dcab00-0c8f-11eb-9134-2e687c303e65.png)
