# python-api-challenge

API assignment associated with class. Uses OpenWeather, Google Places, and Google Maps APIs. 04/16/2021.

--------------------------------------------------------------------------------

The assignment pulls 500+ random latitudes and longitudes, then finds the closest city. 
Using OpenWeather API, current weather data is pulled for each city and relevant values are pulled into a dataframe.
Scatter plots were generated for the overall max temperature vs latitude, humidity vs latitude, cloudiness vs latitude, and wind speed vs latitude.
The data was then split into the northern and southern hemispheres, then the same scatter plots were generated, but this time for each hemisphere individually.
Linear regressions were run on the hemisphere scatter plots.

The dataframe created from the OpenWeather API was pulled into a new document, where the city locations and humidities were used by Google Maps to create a heat map.
From there, the cities were narrowed down to find "ideal" weather conditions for a "vacation".
These ideal locations were run through Google Places to find the first hotel that came up.
The hotel's name was added to the dataframe for the ideal cities.
Markers were added to the heat map for these hotels, with info boxes that showed their names, cities, and countries.

--------------------------------------------------------------------------------

Requires Jupyter Notebook, Python, Matplotlib, json.
