# World_Weather_Analysis

# Background
In this project we are tasked to do the following:

Task: Collect and analyze weather data across cities worldwide.
   
Purpose: PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.
   
Method: Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This process will entail collecting, analyzing, and visualizing the data. Your analysis of the data will be split into three main parts, or stages.

**Collect the Data**
Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
Use the citipy module to list the nearest city to the latitudes and longitudes.
Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
Parse the JSON data from the API request.
Collect the following data from the JSON file and add it to a DataFrame:
 - City, country, and date
 - Latitude and longitude
 - Maximum temperature
 - Humidity
 - Cloudiness
 - Wind speed

**Exploratory Analysis with Visualization**

Create scatter plots of the weather data for the following comparisons:
 - Latitude versus temperature
 - Latitude versus humidity
 - Latitude versus cloudiness
 - Latitude versus wind speed
Determine the correlations for the following weather data:
 - Latitude and temperature
 - Latitude and humidity
 - Latitude and cloudiness
 - Latitude and wind speed
Create a series of heatmaps using the Google Maps and Places API that showcases the following:
 - Latitude and temperature
 - Latitude and humidity
 - Latitude and cloudiness
 - Latitude and wind speed

**Visualize Travel Data**

Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:

   Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
   Create a heatmap for the new DataFrame.
   Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
   Store the name of the first hotel in the DataFrame.
   Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.


# Deliverable 1: Retrieve Weather Data

Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data you gathered in this module, use your API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.

**Deliverable 1 Requirements are as follows:** 

  1. Retrieve all of the following information from the API call: 
       - Latitude and longitude
       - Maximum temperature
       - Percent humidity
       - Percent cloudiness
       - Wind speed
       - Weather description (for example, clouds, fog, light rain, clear sky)
       
   2. Add the weather data to a new DataFrame 
   3. Export the DataFrame as WeatherPy_Database.csv into the Weather_Database folder 

# Deliverable 2: Create a Customer Travel Destinations Map

Use input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

**Deliverable 2 Requirements are as follows:** 

   1. Input statements are written to prompt the customer for their minimum and maximum temperature preferences.
   2. A new DataFrame is created based on the minimum and maximum temperature, and empty rows are dropped.
   3. The hotel name is retrieved and added to the DataFrame, and the rows that don’t have a hotel name are dropped.
   4. The DataFrame is exported as a CSV file into the Vacation_Search folder and is saved as WeatherPy_vacation.csv.
   5. A marker layer map with pop-up markers for the cities in the vacation DataFrame is created, and it is uploaded as a PNG. Each marker has the following information:
        - Hotel name
        - City
        - Country
        - Current weather description with the maximum temperature
   6. The marker layer map is saved and uploaded to the Vacation_Search folder as WeatherPy_vacation_map.png.

# Deliverable 3: Create a Travel Itinerary Map

Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.

**Deliverable 3 Requirements are as follows:** 

   1. Four DataFrames are created, one for each city on the itinerary.
   2. The latitude and longitude pairs for each of the four cities are retrieved.
   3. A directions layer map between the cities and the travel map is created and uploaded as WeatherPy_travel_map.png.
   4. A DataFrame that contains the four cities on the itinerary is created.
   5. A marker layer map with a pop-up marker for the cities on the itinerary is created, and it is uploaded as WeatherPy_travel_map_markers.png. Each marker has the following information:
        - Hotel name
        - City
        - Country
        - Current weather description with the maximum temperature

