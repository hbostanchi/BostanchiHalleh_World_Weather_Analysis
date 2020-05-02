# Next_Trip_Plan

## Project Overview
In this module, we’ll practice our analysis, visualization, and statistical skills by retrieving and analyzing weather data for a hypothetical travel company, PlanMyTrip. Successfully completing the tasks will draw on our knowledge of Python, decision and repetition statements, data structures, Pandas, Matplotlib, and SciPy statistics.
## Resources
-	Data Source: https://openweathermap.org/api
Mapping_Earthquakes
-	Software: Jupyter Notebook, Pandas Library, CityPy, Python Request, APIs, JSON Traversals
## Summary
By the end of this module, we will be able to:
_ Perform tasks using new Python libraries and modules.
_  Retrieve and use data from an API “get” request to a server.
_  Retrieve and store values from a JSON array.
_ Use try and except blocks to resolve errors.
_ Write Python functions.
_ Create scatter plots using the Matplotlib library, and apply styles and features to a plot.
_ Perform linear regression, and add regression lines to scatter plots.
_ Create heatmaps, and add markers using the Google Maps API.
## Challenge Overview
For the new modifications to the PlanMyTrip app, we are asked to add more data to the database, or cities DataFrame, so that customers know the weather in the cities when they click on a pop-up marker. We also added the amount of rainfall or snowfall within the last three hours so that customers can filter the DataFrame using input statements based on the temperature range and whether or not it is raining or snowing. Finally, we created a directions layer Google map that shows the directions between multiple cities for travel.
## Objectives:
-	Use nested try-except blocks
-	Use Pandas methods and attributes on a DataFrame or Series.
-	Create a new DataFrame from a new API search with new weather parameters.
-	Filter DataFrames based on input and nested decision statements, and logical expressions.
-	Create pop-up markers on a Google map from a filtered DataFrame.
-	Add a directions layer on a Google map between cities in the filtered DataFrame.
## Challenge Summary
### part) Get the Weather Description and Amount of Precipitation for Each City
We generated a set of 1,500 random latitudes and longitudes.
Got the nearest city using the citipy module.
Performed an API call with the OpenWeatherMap.
Retrieved the following information from the API call:
-	Latitude and longitude
-	Maximum temperature
-	Percent humidity
-	Percent cloudiness
-	Wind speed
-	Weather description (e.g., clouds, fog, light rain, clear sky)
-	Using a try-except block, if it is raining, get the amount of rainfall in inches for the last three hours. If it is not raining, add 0 inches for the city.
-	Using a try-except block, if it is snowing, get the amount of snow in inches for the last three hours. If it is not snowing, add 0 inches for the city. Added the data to a new DataFrame.
Our new DataFrame looks similar to the following image:
WeatherPy_challenge DataFrame
### Part 2)Have Customers Narrow Their Travel Searches Based on Temperature and Precipitation
We imported the WeatherPy_vacation.csv file from Part 1 as a new DataFrame. Filter the DataFrame for minimum and maximum temperature preferences, and if the rain or snow accumulation is 0 inches or not using conditional statements. Doing the following:
-	Prompt the customer for the minimum temperature preference.
-	Prompt the customer for the maximum temperature preference.
-	Prompt the customer to answer if he or she would like it to be raining or not, using input("Do you want it to be raining? (yes/no) ").
-	Prompt the customer to answer if he or she would like it to be snowing or not, using input("Do you want it to be snowing? (yes/no) ").
Our new hotel DataFrame looks similar to the following image:
### WeatherPy_challenge DataFrame

From the filtered DataFrame we added the cities to a marker layer map with a pop-up marker for each city that includes:
- Hotel name
- City
- Country
- Current weather description with the maximum temperature

### Part 3)Create a Travel Itinerary with a Corresponding Map
We created a map (travel itinerary) that shows the route between four cities from the customer’s possible travel destinations, and then created a map with pop-up markers for the four cities, by:
Importing the WeatherPy_vacation.csv file as a new DataFrame. From the vacation search map, we chose four cities in close proximity on our map that are on the same continent that a customer might travel to, and then created a directions layer map.
- We Filtered the DataFrame for each city we wanted to go to and created separate DataFrames for each city.
- Used the directions Layer instructions from the gmaps documentation
- Use the list indexing and Pandas methods to get the latitude-longitude pairs for each city DataFrame as tuples.

For the travel_mode, we used either DRIVING, BICYCLING, or WALKING.

# View [Live Demo](https://hbostanchi.github.io/Next_Trip_Plan/) Next_Trip_Plan
