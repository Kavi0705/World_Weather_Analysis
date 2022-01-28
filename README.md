# World_Weather_Analysis

## Background & Purpose
A travel techonolgy company, PlanMyTrip, would like to develop an app for customers to use in order to recommend hotels based on client preferences, including weather conditions. Beta testers will enter responses to input statements to filter for their particular weather preferences, which then will be used to recommend potential travel destinations and nearby hotels. From the list of these potential travel destinations, the beta testers will then choose 4 cities to help create a travel itinerary.

## Results
### Retrieve Weather Data
The first step was to generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call to retrieve the following information: latitude, longitude, maximum temperature, percent humidity, percent cloudiness, wind speed, and current weather description.

<img width="611" alt="City_Data_df" src="https://user-images.githubusercontent.com/93743169/151635760-1daa2e4f-3c32-415d-926e-ce9d9c92f3fa.png">

### Create a Customer Travel Destinations Map
Then, using input statements were used to obtain customer weather preferences to identify potential travel destinations and nearby hotels. 

<img width="602" alt="Hotel_df_based on temp preference" src="https://user-images.githubusercontent.com/93743169/151636014-2806f448-9d38-426a-98fb-62f5ca1558c4.png">

Based on this information, a layer map was generated, with pop-up markers, for the cities, which includes inforamtion on hotel name, city, county, and the current weather description with maximum temperature.

<img width="603" alt="WeatherPy_vacation_map" src="https://user-images.githubusercontent.com/93743169/151636036-e6be0085-b873-4f14-82c8-9e1b8403408f.png">

### Create a Travel Itinerary Map
Finally, the Google Directions API was utilized to create a travel itinerary that shouls the route between 4 chosen cities from the customer's possible travel destinations.

<img width="960" alt="WeatherPy_travel_map" src="https://user-images.githubusercontent.com/93743169/151636351-462acc6b-0dca-4301-8fe4-001abe9beddb.png">

Then, another layer map was generated, with pop-up markers,for each city that displayed hotel name, city, county, and the current weather description.

<img width="1260" alt="WeatherPy_travel_map_marker" src="https://user-images.githubusercontent.com/93743169/151636480-d5b7007d-b61f-4a4f-be22-19d05384d3c5.png">

## Summary
This method can be applied to any location within the world given customer's preferences. Additional code can be added to include parameters such as finding nearby restaurants, or museums. The code can also be altered if itinerary needed to be changed for someone who is biking or walking. This code allows one to glean a lot more detailed information than just a plain search using Google Maps would.


