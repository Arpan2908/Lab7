# Lab7 - Geoparsing with Python

This exercise works on geoparsing which is extracting the names of places from texts and assigning those names with coordinates for the spatial understanding. This code uses libraries including geopandas, nltk, matplotlib.pyplot and others to extract the names of cities from books and map these places on the map and graph based on the number of times they occur in the text. 

The gazetteer we are using is appropriate for the text as it contains the name of the country and the latitudes and longitudes of our city. Nominatim requires an email address to be used. There are also some challenges of using Nominatim with a book published in 1859 as there are a lot of cities with different names than what it used to be back in 1859. For example, Bombay is now Mumbai, Calcutta is now Kolkata etc., so using the new names might not allow us to extract spatial information during geoparsing. 

The outputs are not fully accurate. The words like ‘Of’, ‘much’ and ‘man’ are considered as a city name which probably is not intended to describe a place in the book. 

Another approach to mapping this data is using graduated color composite. A count could be set up for each time a name comes up in the text and then different shades of a color instead of opacity could be used as it could be hard to figure out the city if it comes only once or twice if we use the opacity to map places. 

