# World_Weather_Analysis
This Read Me Contains: 1 - Project Description 2 - List of outputs: files and pictures.

1 - Project Description

Module G6 Challenge:  WeatherPy. 
	• Generate random latitudes and longitudes and use them to pull cities from citipy library. 
	• Make API calls to OpenWeatherMap to pull Weather data based on lats and lngs.
	• Use inputs on weather preferences to crawl Google Nearby Search for related data
	• Plot a Google map showing cities meeting preferences, with a marker layer
	• Use Google Direction Layers to plot a map of selected cities
	• Use Google Marker Layers to plot info for selected vacation cities.
	
	Part I. Get the Weather Description and Amount of Precipitation for Each City
1.2.a Add the latitudes and longitudes to a list.
1.3.Get the nearest city using the citipy module. 
1.4-5.Perform an API Call with the OpenWeatherMap.
         Return: Latitude and Longitude, Max Temp, Percent Humidity, Percent Cloudiness,    Wind,Speed, Weather description  
       Return: Rainfall -use try-except, if it is raining get rainfall # in last three hours. If not raining, add 0 for city
        Return: Snow -use try-except, if it is snowing get snowfall # in last three hours. If not snowing, add 0 for city    
1.6. Add collected data to new dataframe
1.7. Save new DataFrame as CSV to be used later in Part II.  weatherPy_challenge.csv
1.8. Git hub 
1.9. ?? Using Pandas: How many cities have recorded rainfall or snowfall

Part II. Provide inputs for customers to narrow Travel Searches based on Temp and Rain
2.2 Import Weather Data CSV as new Dataframe.
2.3 Filter the DF for minimum and max temps and if rain or snow accumulation is - inches using conditionals
2.3a Prompt Customer for Min Temperature Preference
2.3b Prompt Customer for Max Temperature Preference
2.3c Prompt Customer for Rain Preference
2.3d Prompt Customer for Snow Preference
2.4 Add the cities to a marker layer map with pop-marker for each city that includes:
2.4   Hotel name, City, Country, Current Weather Descrip with Max Temp
2.4a  Create the Hotel DF.  
2.4b  Configure search parameters 
2.4c  Crawl through Google NearbySearch to get data based on our locations
2.4d  Iterate through the DataFrame by row, and populate the info_box_template
2.5  Save and upload new DF as WeatherPy_vacation.csv
2.6  Save and upload new marker layer map as WeatherPy_vacation_map.png

Part III. Create a Travel Itinerary with a Corresponding Map
3.1 Create new Jup NB as Vacation_Itinerary
3.2 Import WeatherPy_vacation.csv as new DF
3.3 From the vacation search map,  choose at least four cities in close proximity on your map that are on the same continent that customer may like  and create a directions layer map.
3.4 Create needed dataframes. One per city and one with all the filtered cities.   Use list indexing to get the latitude and longitude pairs
3.5 Create the WeatherPy_travel_map.png
3.6 Create the marker layer travel map as WeatherPy_travel_map_markers.png
3.6.1    use info_box_template and iterate thru df to op info_box_template
3.6.2    Create the marker layer travel map


2 - List of outputs: files and pictures.
Code: 
	1 Weather_Database.ipynb
	 2 Vacation_Search.ipynb
	 3  Vacation_Itinerary.ipynb
CSV Files: 
	1 Weather_Py_challenge.csv
	2 Weather_Py_vacation.csv
	
Image Files: 
	1  WeatherPy_vacation_map.png 
	2  WeatherPy_travel_map.png
	3  WeatherPy_travel_map_markers.png
