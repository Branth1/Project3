# Project3
Shared Colab Link:
https://colab.research.google.com/github/Branth1/Project3/blob/master/Project3.ipynb

GitHub Link:
https://github.com/Branth1/Project3
## Description

This is a study of the data collected by the Bulk Meteorology Instrument Package which measuresa variety of parameters that characterize weather conditions above the sea surface at two different sites from the OOI database. 

The data sets being studied and compared are the wind speeds and precipitation rates for two different sites. The following analysis will look at the data from these sites and determine if there is any relation between the two. Can we use data from one site to predict data at the other? 

It should be noted that there may exist an error in the Correlated analysis of the Oregon Shelf Surface Mooring Data. Although attempts have been made to verify this data, further testing would be needed to confirm or disprove the accuracy of the analysis.

## Background

**The questions we are looking to solve are as follows:**

        1-Is there any relation between the windspeed and rain rate at each site?

        2-Is there any correlation between the wind at one and the other?

        3-Is there any correlation between the rain at one site and the other?

        4-What patterns if any can be seen between the average rain rate at both sites?

        5-What patterns if any can be seen between the average wind speed at both sites?

**The sites and dates for recording are as follows:**

Oregon Shelf Surface Mooring

Oregon Offshore Surface Mooring

All Data Was Collected Between Jan 01, 2019 and Jan 01, 2020

For additional information on the instruments used please see the link to the code above.

## Solution/Results

The data was analyzed utilizing the code found in the link above. First the data was requested from the OOI website and the rain rate and wind speed for each site were analyzed:
**Initial Data Analysis**
Note: For the following graphs, the vertical bands have been added to further clarify trends at each site:

        Blue = No wind or Rain

        Green = Wind but No Rain

        Red = Rain and No Wind

        Yellow = Rain and Wind
        
**Oregon Shelf Surface Mooring**

![](https://github.com/Branth1/Project2/blob/master/Oregon%20Shelf%20Data.png?raw=true)

**Oregon Offshore Surface Mooring**

![](https://github.com/Branth1/Project2/blob/master/Oregon%20Offshore%20Data.png?raw=true)

**Cross-Correlation of Wind Speed**

Note: Max Lag = -2971 @ Correlation Value = 0.0857

![](https://github.com/Branth1/Project2/blob/master/Coorelation%20Wind%20(lag-2971)(0.0857).png?raw=true)

**Cross-Correlation of Rain Rate**

Note: Max Lag = 1 @ Correlation Value = 0.4306

![](https://github.com/Branth1/Project2/blob/master/Coorelation%20Rain(0.4306)lag(1).png?raw=true)

**Monthly Average Wind Speed**

![](https://github.com/Branth1/Project2/blob/master/Average%20Wind.png?raw=true)

**Monthly Average Rain Rate**

![](https://github.com/Branth1/Project2/blob/master/Average%20Rain.png?raw=true)

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

Data was downloaded from OOI:
https://oceanobservatories.org
