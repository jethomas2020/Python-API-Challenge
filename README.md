# Python-API-Challenge

-------------------------
# What's the Weather Like?

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. We'll take a look at Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: "Duh. It gets hotter..."

But, if pressed, how would you prove it?


![Alt text](equatorsign.png "Equator Sign")




Part I - WeatherPy

In this example, we'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, we'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

We created a series of scatter plots to showcase the following relationships:

    Temperature (F) vs. Latitude
    Humidity (%) vs. Latitude
    Cloudiness (%) vs. Latitude
    Wind Speed (mph) vs. Latitude
    
These plot images are stored within the Output Folder within the WeatherPy Folder. 

After each plot a sentence was added within the Jupyter Notebook file explaining our findings. 

Secondly, we ran linear regressions on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

    Northern Hemisphere - Temperature (F) vs. Latitude
    Southern Hemisphere - Temperature (F) vs. Latitude
    Northern Hemisphere - Humidity (%) vs. Latitude
    Southern Hemisphere - Humidity (%) vs. Latitude
    Northern Hemisphere - Cloudiness (%) vs. Latitude
    Southern Hemisphere - Cloudiness (%) vs. Latitude
    Northern Hemisphere - Wind Speed (mph) vs. Latitude
    Southern Hemisphere - Wind Speed (mph) vs. Latitude

Within the Jupyter Notebook file, after each pair of plots we explained what the linear regression is modeling and any relationships noticed as part of our analysis.

Our final notebook includes:

    Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
    Perform a weather check on each of the cities using a series of successive API calls.
    Include a print log of each city as it's being processed with the city number and city name.
    Save a CSV of all retrieved data and a PNG image for each scatter plot. (Images saved in the Output and Output2 Folders within the WeatherPy folder) 


------------------------------------    
# Part II - VacationPy

We'll use skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.

    Create a heat map that displays the humidity for every city from the part I of the homework.

    Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

    Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

    Hotel map
