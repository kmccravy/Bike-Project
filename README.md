# Amsterdam and Seattle Bike Network Comparison

### Project by: Kelsey McCravy

#### Summary

For my final project, I am comparing bike assessibility connectivity using network analysis of Amsterdam's and Seattle's bike network. From my expereince on my study abroad last summer, Amsterdam has a great bike network that allows access to all the of city. I want to see how a city in the United States compares, and I went with Seattle, Washington due to it similar size to Amsterdam.

#### Questions and Objectives

Questions: Which city has a bike network that connects more areas around the city? In which city does it take less time to bike around and access different parts of the city?
Objective: To understand how much of the city is connected through the bike network. To understand how long it takes to access different parts of the city from the city center.

#### Datasets

[Amsterdam bike network dataset](https://maps.amsterdam.nl/fietsnetten/)

[Amsterdam city limits polygon](https://maps.amsterdam.nl/gebiedsindeling/)

[Seattle bike network dataset](https://www.arcgis.com/apps/mapviewer/index.html?layers=bf36bd11b499489d8cc1d491b72eb712)

[Seattle city limits polygon](https://data-seattlecitygis.opendata.arcgis.com/datasets/4fbe28084541458e9b393b112ff76e86_0/explore)


#### Python Packages

The current Python packages I know will need are the ones needed to for assignment 3 and the netwrok run-through. These are geopandas, osmnx, networkx, os, shapely, descartes, numpy, matplotlib.pyplot, folium. I am still doing research on which packages I need to convert my GeoJSONs to graph dataset. Based on [this](https://networkx.org/documentation/stable/auto_examples/geospatial/plot_lines.html) documentation from Networkx, I also need momepy, contextily, and libpysal.

#### Planned Approach

To compare the bike network of Amsterdam and Seattle, I will do an analysis similar to Assignment 3. I will produce an isochrone map of each bike network and analyze how much of the city can be accessed by bike and how long it takes to access different parts of the city.
To better understand how much area of the city is connected by the bike network, I will create a 400 meter buffer (about .25 miles). I will find the percentage of the city that is contained within the buffer to analyze my first question. 
To analyze my second question, I will first convert my data into a graph dataset with edges and nodes. Using the coordinates of the city center given by Google Maps, I will create  isochrone polygons and a map to see how long it takes to access the city from the city center. My proccess will be the same to the one in the [network data analysis example](https://cleo-lab.github.io/gds-applications-site/lectures/week3/lecture-3.html#) on the GEOG 490 course website. I will then use the polygons created for each time to calculate the percentage of the city that is accessibily from the city center within that time.

#### Expected Outcomes

I expect Amsterdam to have a higher percentage of the city accessible by bike. Additionally, I believe more of the city will be accessible than Seattle at lower times.
