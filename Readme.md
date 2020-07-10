## Clustering Neighbhorhoods in Toronto, CAN

The goal of this analysis is to identify and cluster similar neighborhoods in Toronto CAN based on their proximity to desirable venues.

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

