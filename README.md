# Project3
Shared Colab Link:
https://colab.research.google.com/github/Branth1/Project3/blob/master/Project3.ipynb

GitHub Link:
https://github.com/Branth1/Project3
## Description

This is a study of the data collected by the United States Geological Survey group (USGS) from January 01 2010 through February 22, 2020. All seismic data being observed has been filtered with a minimum magnitude of 2.5. 

The USGS collects a wide range of data on earthquakes, faults and crustal deformation to increase our understanding of earthquake source processes, occurrence, and effects; and synthesize this knowledge into probabilistic seismic hazard assessments, aftershock forecasts, and ground-shaking scenarios for anticipated major earthquakes.

The data sets being studied and compared are the magnitudes compared to time and location. The following analysis will look at the data from first a wide range pacific ocean view coordinate with a coordinate window:

longitude range (-152.93 to -115.66) and latitude range (33.45 to 56.47).

This is followed by a focus on the affects measured in April 2015 and concluded with a focus on the divergent and transform tendencies as seen around the juan de fuca plate. This coordinate window is:

longitude range (-135 to -115) and latitude range (40 to 55).

For a closer look at the work being conducted by the USGS or for further information, their website can be found in the reference section below.
## Background

**The questions we are looking to solve are as follows:**

        1-Across what geographic area are we able to observe earthquake data in the map?

        2-Why are most of the earthquakes in that area?

        3-What is the range and magnitude of the earthquake size in this area?

        4-Where are earthquakes located in April 2015 and what event can be linked to these? 

        5-What patterns are observed in magnitude and location over time for a transform and divergent boundary region?

**The Data used for analysis is:**

Initial Bulk Data set:

https://earthquake.usgs.gov/fdsnws/event/1/query.csv?starttime=2010-01-01%2000:00:00&endtime=2020-02-22%2023:59:59&maxlatitude=56.472&minlatitude=33.445&maxlongitude=-115.664&minlongitude=-152.93&minmagnitude=2.5&orderby=time

Refined Juan De Fuca Plate Data set:

https://earthquake.usgs.gov/fdsnws/event/1/query.csv?starttime=2010-01-01%2000:00:00&endtime=2020-02-22%2023:59:59&maxlatitude=55&minlatitude=40&maxlongitude=-115&minlongitude=-135&minmagnitude=2.5&orderby=time

All Data Was Collected Between Jan 01, 2010 and Feb 22, 2020

For additional information on the analysis used please see the link to the code above.

## Solution/Results

The data was analyzed utilizing the code found in the link above. First the bulk data set was requested and the magnitude was plotted against time.
**Initial Data Analysis**
Note: For the following graphs, a screen shot is shown. To view the interactive map please visit the link to the colab page above. In all graphs, the magnitude of earthquake is referenced by the size of the marker.

**Bulk Data Scatter Plot**

![](https://github.com/Branth1/Project3/blob/master/Bulk%20Scatter.png?raw=true)

**Bulk Data Map**

![](https://github.com/Branth1/Project3/blob/master/Bulk%20Map.png?raw=true)

**Interactive Map**

Note: In the live version, the years visible can be filtered by clicking on the legend. Hovering over the indicator will display the coordinates, date and magnitude.

![](https://github.com/Branth1/Project3/blob/master/Interactive%20Map.png?raw=true)

**April 2015 Map**

![](https://github.com/Branth1/Project3/blob/master/April%202015.png?raw=true)

**Juan De Fuca Plate Scatter Plot**

![](https://github.com/Branth1/Project3/blob/master/Juan%20De%20Fuca%20Scatter.png?raw=true)

**Juan De Fuca Plate Map Plot**

![](https://github.com/Branth1/Project3/blob/master/Juan%20Map.png?raw=true)

## Conclusions
From the analysis conducted, the following conclusions were made:

* When looking at the first two plots, we can see that majority of the time throughout the year these sites experience wind but no rain. When analyzing the data, it was normalized, and the significance of wind/ rain values was set to exclude anything that was under 30%. From these graphs we can also see that there are minimal times of rain without wind in either site.  

* Now looking at the correlation graph, we can see the possible error described earlier in the wind graphs. However, if we infer that the data were to follow similar trends to what is visible, it can be said that there is truly a minimal correlation for the wind between the two sites. The max correlation value for wind is seen to be 0.0857, indicating a nonexistent relationship between the two sets of data. Not to mention the fact that the time delay is about 18 weeks. These sites are only about 36.7 miles from each other. This makes some sense considering the previous graphs showed that these sites are typically always windy. 

* However, when we interpret the correlation graph for rain rate, we get a slightly different result. The highest correlation occurring with a lag of one hour and a max correlation value of 0.4306. Although this is still a fairly low relationship strength, I believe it would warrant further testing. From this we can say that the Oregon Shelf experiences similar rain rates about an hour after the Oregon Offshore location with some a correlation factor of 0.4306.
There does not appear to be any relation between the time lag for wind speed and rain rate. It seems to always be windy at these two sites. 

* When we look at the figure showing the average wind speed for the year a few things can be noticed. Although there did not appear to be any trend to wind from site to site, we can see there is a trend throughout the year. Both sites follow the same average wind patterns. The highest occurring in January, decreasing until about April before dropping to the lowest point of the year in August. It then increases back up going into winter. However, the highest wind rate is still seen in January at the Oregon Offshore site with a speed of about 6.7 m/s. 

* Finally looking at the average rain rate between each site. It can again be seen that there appears to be a strong relationship between the patterns of each site throughout the year. The highest rain rate occurs around early February and will begin decreasing with a few spikes until the lowest values seen in early August, late July. It then peaks again in early September. The highest rain rate appears to be about 0.13 mm/hr and the lowest about 0.01 mm/hr. 

* When taking both of these into consideration it would appear that August is the calmest time of year with the least wind and rain at both sites. Although we did not see a correlation for wind with the analysis as performed, this would have occurred during the area that is missing in the wind correlation graph. This is a good example as to why variations of data analysis should be performed. 

## References

Data was downloaded from USGS:
https://earthquake.usgs.gov

Map Images are from:
https://www.openstreetmap.org

April 2015 Earthquake information:
