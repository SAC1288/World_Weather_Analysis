# World Weather Analysis Project

Created a PlanMyTrip app whereby any user can input the type of weather conditions they seek and the app will return specific destinations that meet her criteria. In addition, the user can use the app to plan her trips as it will return the location of specific hotels the user can stay at within her desired destinations.

The app works by first collecting 2,000 pieces of location data across the globe and then filters through the data through the nearest.city method to come up with about 700 cities that we can analyze. We then requests weather data from the google weather maps API and store the infromation for all 700 cities in a separate list along with the names of those cities and their locations. Once we have this information, we then create a dataframe from the list and then export to a separate csv file so that it can accomplish additional tasks as requried by the app.

Once the CSV file is created, the user is then prompted to enter the range of max temperatures for the destinations she wishes to visit. This algorithm can be claibrated to allow the user to enter other types of information aside from max temperature (for example, cloudiness, windspeed, etc.). Once the user sepcifies the weather conidtions, then the city list is further condensed to enlist locations that meet the user's weather requirements. 

The algorithm then uses Google Maps API to find nearby lodging for the user for each of the cities within the newly condensed list. This list is created in a new dataframe and then exported to a new csv, which is then used to perform the final functions of the app. Note, a map with markers is produced to show the user all the lodging locations that meet his or her weather criteria.

Once the user has the lodging information, then she can plan her trip. She does this by selecting which lodging locations in the cities that she wants to travel to and then tells the app what are her startting and ending locations. Once she finishes inputting her route, the app will display a map of her route with distance data and markers that detail information about each hotel that she will be lodging. 


