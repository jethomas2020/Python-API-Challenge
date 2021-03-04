# Python-API-Challenge

-------------------------
# What's the Weather Like?

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. We'll take a look at Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: "Duh. It gets hotter..."

But, if pressed, how would you prove it?


![Alt text](equatorsign.png "Equator Sign")



----------------------------
# Part I - WeatherPy

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
    Save a CSV of all retrieved data and a PNG image for each scatter plot. 
    (Images saved in the Output and Output2 Folders within the WeatherPy folder) 

---------------------
## For Part I,  a few observable trends based on the data:

1. In the scatter plot for City Latitude vs. Maximum Temperature above, as cities are closer to the equator (where latitude is 0 degrees), the higher the maximum temperature.

2. In the scatter plot for City Latitude vs. Humidity above, there is no strong correlation that can be seen. The data does show that cities that are in the Northern Hemisphere (latitude >0 degree) tend to have a stronger cluster of higher humidity percentages as it nears the North Pole. 

3. In the scatter plot for City Latitude vs. Cloudiness above, there is no strong correlation that can be seen. The data does show scattered clusters of higher cloudiness percentages at the top right and bottom right, as well as top left, without being able to draw strong conclusions.

4. In the scatter plot for City Latitude vs. Wind Speed above, there is no strong correlation that can be seen. 
The data does show clusters of higher wind speed (mph) at the bottom of the chart across the spectrum of city latitudes without being able to draw strong conclusions. The majority of the wind speeds overall appear to 15mph or less. One oulier at >40mph is visible at around 70 degrees latitude closer to teh North Pole.


------------------------------------    
# Part II - VacationPy

Next, we'll expand our efforts in working with weather data to plan future vacations. We'll use jupyter-gmaps and the Google Places API for this part of the assignment.

We will further:


    Create a heat map that displays the humidity for every city from the part I of the project. 
   

Narrow down the DataFrame to find our ideal weather condition. For example:

    A max temperature lower than 80 degrees but higher than 70.

    Wind speed less than 10 mph.

    Zero cloudiness.

    Drop any rows that don't contain all three conditions. We want to be sure the weather is ideal.

 

Used Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
    
