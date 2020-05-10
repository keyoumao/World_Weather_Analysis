# World_Weather_Analysis
## Challenge
### Part 1 Instructions
Get the Weather Description and Amount of Precipitation for Each City
To complete this task, follow these steps:

Create a new Jupyter Notebook file and name it Weather_Database.ipynb.
Generate a new set of 1,500 random latitudes and longitudes.
Get the nearest city using the citipy module.
Perform an API call with the OpenWeatherMap.
Retrieve the following information from the API call:
Latitude and longitude
Maximum temperature
Percent humidity
Percent cloudiness
Wind speed
Weather description (e.g., clouds, fog, light rain, clear sky)
Using a try-except block, in the try block if it is raining, get the amount of rainfall in inches for the last three hours. In the except block handle the KeyError if there is no rainfall and add 0 inches for the rainfall amount.
Using a try-except block, in the try block if it is snowing, get the amount of snowfall in inches for the last three hours. In the except block handle the KeyError if there is no snowfall and add 0 inches for the snowfall amount.
Add the data to a new DataFrame.
Save the new DataFrame as a CSV file to be used for Part 2.
Upload the CSV file as part of your submission as WeatherPy_challenge.csv.
Answer this question using Pandas methods: How many cities have recorded rainfall or snow?
For our data is 0 because of the temperature limit. 

The new cities_data DataFrame summarizes the current weather description, and rain and snow in inches for the last three hours.

### Part 2 Instructions
Have Customers Narrow Their Travel Searches Based on Temperature and Precipitation
To complete this task, follow these steps:

Create a new Jupyter Notebook file and name it Vacation_Search.ipynb.
Import the WeatherPy_vacation.csv file from Part 1 as a new DataFrame.
Filter the DataFrame for minimum and maximum temperature preferences, and if the rain or snow accumulation is 0 inches or not using conditional statements. Do the following:
Prompt the customer for the minimum temperature preference.
Prompt the customer for the maximum temperature preference.
Prompt the customer to answer if he or she would like it to be raining or not, using input("Do you want it to be raining? (yes/no) ").
Prompt the customer to answer if he or she would like it to be snowing or not, using input("Do you want it to be snowing? (yes/no) ").
Add the cities to a marker layer map with a pop-up marker for each city that includes:
Hotel name
City
Country
Current weather description with the maximum temperature
Save and upload the new DataFrame as WeatherPy_vacation.csv.
Save and upload the new marker layer map as WeatherPy_vacation_map.png.

The new hotel DataFrame has the Hotel Name column completed where hotels are found.

The marker layer map shows markers for each city in the new hotel DataFrame.

The new hotel DataFrame includes pop-up markers for each city.

### Part 3 Instructions
Create a Travel Itinerary with a Corresponding Map
Finally, you will create a map (travel itinerary) that shows the route between four cities from the customer’s possible travel destinations, and then create a map with pop-up markers for the four cities. To complete these tasks, follow these steps:

Enable the “Directions API” in your Google account for your API key.
On the Google Cloud Platform, select APIs from the left-hand side.
Viewing the options on the Google Cloud Platform
Then, select "Directions API."
Viewing the APIs on your Google Account
Click “Enable” on the Directions API. 
 Viewing the APIs on your Google Account. 
Create a new Jupyter Notebook file and label it Vacation_Itinerary.ipynb.
Import the WeatherPy_vacation.csv file as a new DataFrame.
From the vacation search map, choose at least four cities in close proximity on your map that are on the same continent that a customer might travel to, and then create a directions layer map.
Hints:

Filter the DataFrame for each city you want to go to and create separate DataFrames for each city.
Use the directions Layer instructions from the gmaps documentation (Links to an external site.).
Use the list indexing and Pandas methods to get the latitude-longitude pairs for each city DataFrame as tuples.
For the travel_mode, use either DRIVING, BICYCLING, or WALKING.
Hint: If the cities are too far apart, some travel modes will not be available.
Take a screenshot of the route and save it as WeatherPy_travel_map.png.
Create a marker layer map for the four cities.
Hint: Create a new DataFrame that has all the individual city DataFrames you created.

On the marker layer map, make sure each city has a pop-up marker that contains the following:
Hotel name
City
Country
Current weather description with the maximum temperature
Take a screenshot of the marker layer map for the route and save it as WeatherPy_travel_map_markers.png.

### Please find the corresponding files for this challenge:

**Code for Parts 1, 2, and 3 of the challenge.**<br />
Weather_Database.ipynb.
Vacation_Search.ipynb
Vacation_Itinerary.ipynb

**A “data” folder containing the following CSV files.**<br />
WeatherPy_challenge.csv
WeatherPy_vacation.csv

**An “image” folder containing the images of your maps for Parts 2 and 3.**<br />
WeatherPy_vacation_map.png
WeatherPy_travel_map.png
WeatherPy_travel_map_markers.png
