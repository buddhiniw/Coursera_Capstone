## Clustering Neighbhorhoods in Toronto, CAN

##### Scenario: 
I live in Toronto, CAN (hypothetically) in the neighborhood of Humber Summit. I get a job offer from a company based in Toronto city making it nessasary for me to find a neighborhood near my new work place. I love my old neighborhood and all the ammenties it offered. So now I am on the hunt for a neighborhood near my new workplace that is similar to my old neighborhood. How should I go about doing that? 

##### Solution:
Make a list of things I like about my old neighborhood. Prioratize. Lets say I love all the restaurants (: ) ). Now I have to find a neighborhood that allow easy access to similar restaurants.

So the goal of this analysis is to identify and cluster similar neighborhoods in Toronto CAN based on their proximity to desirable venues such as restuarants. 

The datasets:

* Toronto neighborhood data - From wikipedia
* Venue locations and names - Foursquare API


### Methodolgy
* Scrape the wikipedia webpage using Beautifulsoup library to get the neighborhood zipcodes, names and boroughs. 
* Load the data table in to a pandas dataframe
** Clean the dataset (check for nulls, remove null neighborhoods)
* Get the geo spatial data for Toronto and fill the longitude and latitudes of the neighborhoods in the data frame.
* Use follium to display the neighborhood locations in a Toronto map.
* Use the Foursquare API to get venues within 100 mile radius of each neighborhood.
* Clean the dataset.
* Explore the venue dataset:
** Types of venues?
** Venue count for each neighborhood?
** Top 3 venue types in each neighborhood?
* Use follium to display the neighborhoods with marker size corresponding to the number of venues in 100 mile radius. This helps to identify which neighborhoods have more venues in the map easily.

