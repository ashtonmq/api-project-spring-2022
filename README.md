# api-project-spring-2022

The purpose of this project was to create a dynamic, web-based chart using API data of my choice to provide meaningful insight into said data. The data I decided to use for this project was eviction data for NYC (https://data.cityofnewyork.us/City-Government/Evictions/6z8x-wfk4) which was first entered in 2017 and is still being updated daily.

The APIs used in this project were the Image Chart API (https://documentation.image-charts.com/), and the Socrata Open Data API (SODA) which grabbed data from NYCOpenData (https://data.cityofnewyork.us/). SODA provided access to a continually updating .json file which is where I grabbed my data from, and I used the Image Chart API to implement both a pie chart (composition chart) and a line chart (trend chart) to my webpage. The SODA API converted the raw data I was using into a web-accessible .json file, and using JQuery and JavaSCript I was able to comb through that data and send the data I was interested in to the Image Charts API where the charts were created and further implemented into my webpage.

As for the charts I decided to implement:

I chose to implement a line chart as I wanted to identify trends in the number of evictions happening per year in NYC over time, and I chose to implement a pie chart to identify what percentage of all evictions come from each borough.

Using the line chart, I mapped out the total number of evictions each year for the entirety of NYC as points on the graph, and connected them to identify trends (increase, decrease, stay the same) in the number of evictions happening per year. This chart updates dynamically so it will continue to update the position of the data points and add years to the x-axis.

Using the pie chart, I set each of the five boroughs in NYC as a slice in the chart. Again, these chart update dynamically so if for some reason any new boroughs are entered into the database, a new slice will be automatically created. For each slice, I calculated the eviction rate percentages for each borough respectively. This chart makes it easy to identify which boroughs of NYC have the highest eviction rates, lowest eviction rates, and everything in between.


