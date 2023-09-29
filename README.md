## Backgroud

Data allows us to definitively answer questions. This challenge shows the keys that data science holds through a common scientific question, "What is the weather like as we approach the equator?"
Mnay know that as one approaches the equator, it gets hotter. This data science challenge allows you to provide the data to prove this matter.

#### Before you begin
Add a .gitignore file to you repo. This will prevent the *api_keys.py* file that contains your API key from being shared with the public.
  - Open the .gitignore file and type:
          # Adding config.py file.
          api_keys.py
In the command line, type git status and press Enter. The output should indicate that the .gitignore file has been modified and the api_keys.py file is untracked.

# Instructions 
### Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python library, the OpenWeatherMap API, and your problem-solving skills to create a representative model of weather across cities. *https://openweathermap.org/api*
1. Create Plots to Showcase the Relationship Between Weather Variables and Latitude
     - use the OpenWeatherMap API to retrieve weather data from the cities list                 generated in the starter code.
     - create a series of scatter plots to show the follwoing relationships:
           Latitude vs. Temperature
           Latitude vs. Humidity
           Latitude vs. Cloudiness
           Latitude vs. Wind Speed
2. Compute Linear Regression for Each Relationship
    - compute the linear regression for each relationship. Separate the plots into
      Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern
      Hemisphere (less than 0 degrees latitude)
    - create a series of scatter plots. you should include the linear regression line, the model's formulat, and the r-values.
    - create these plots:
        Northern Hemisphere: Temperature vs. Latitude
        Southern Hemisphere: Temperature vs. Latitude
        Northern Hemisphere: Humidity vs. Latitude
        Southern Hemisphere: Humidity vs. Latitude
        Northern Hemisphere: Cloudiness vs. Latitude
        Southern Hemisphere: Cloudiness vs. Latitude
        Northern Hemisphere: Wind Speed vs. Latitude
        Southern Hemisphere: Wind Speed vs. Latitude
### Part 2: VacationPy
In this deliverable, you are observing which cities have ideal weather for future vactions.
1. Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.
2. Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
    - A max temperature lower than 27 degrees but higher than 21
    - Wind speed less than 4.5 m/s
    - Zero cloudiness
3. Create a new DataFrame called *hotel_df* to store the city, country, coordinates, and humidity.
4. For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
5. Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:
