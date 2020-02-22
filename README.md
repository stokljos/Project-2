# Wind-Speed-and-Rain-Rate-in-the-Ocean-Data-Analysis
Code URL: https://github.com/stokljos/Wind-Speed-and-Rain-Rate-in-the-Ocean-Data-Analysis/blob/master/450_Project2.ipynb

Introduction:

The purpose of this project is to look at rain rate and wind speed at various locations in the ocean over an entire year and 
see how seasons or different times of the year affects these variables. The was that rain rate and wind speed can be measured 
is with a Bulk Meteorology Instrument Package. Its main purpose is to measure parameters that have something to do with the wind, 
rain, or surface of the ocean.
The data that will be downloaded is from the OOI website that has a bulk Meteorology Instrument at an Oregon Shelf Surface 
Mooring and an Oregon Offshore Surface Mooring.
  
Procedure (explanation of code):

The code I wrote has 13 cells and I will give a brief description of what each cell does:
Cell 1: Imports relevant packages that I use throughout the code to analysis the data.
Cell 2: Defines the username, token, and urls needed to request data from the website.
Cell 3: The data downloaded counts seconds from January 1st 1900, so in this cell I convert the time to pacific time zone with
the relevant days, months, and year.
Cell 4: I define my lists for wind, rain rate, and time for each site and request the data to append into the correct list.
Cell 5: When a data point is null, it prints out NaN for that point, so this cell converts those points to zeros to get more 
accurate graphs.
Cell 6: Plots the rain rate and wind speed at the Ocean Shelf Surface Mooring site
Cell 7: Plots the rain rate and wind speed at the Ocean Offshore Surface Mooring.
Cell 8 and 9: Creates new lists and finds out at which times during the year is it 1) Rainy and Windy, 2) Rainy but not windy, 
3) Windy but not Rainy, and 4) No wind or rain. This is then plotted on a graph for each site.
Cell 10: Plots the cross correlation for wind speed at each site.
Cell 11: Plots the cross correlation for the Rain Rate at each site.
Cell 12 and 13: Plots the average wind speeds and rain rates for the months for each site.

Data:

Analysis:

1)	Plot the cross-correlation function between wind speed at both sites? (Graphs 5 and 6) What is the highest correlation? 
What is the time lag? 
The highest correlation is 0.7 (70%) and the time lag at the point is zero seconds for wind speed. This means that overall 
throughout the year, the two sites seem to be getting the same wind speed at the same time 70% of the time.
2)	Plot the cross-correlation function between rain rate at both sites? (Graphs 7 and 8) What is the highest correlation? 
What is the time lag?
The highest correlation is 0.6 and the time lag at that point is zero seconds for rain rate. Just like wind speed, 
the sites are experiencing the same rain rate about 60% the time with no time lag. 
3)	Is there any relationship between the time lag of wind speed and rain rate?
Yes, there seems to be a relationship. Both graphs showed that there is no time lag for 60-70% of the time at both sites.
Due to the high cross correlations for both wind speed and rain rate, it is assumed that both of the sites are close enough 
together that they are experiencing the same weather throughout the year.
4) In another plot, calculate and plot the monthly average of the wind speed and rain rate for each site (Graphs 9 and 10)
•	What pattern do you see? Explain.
  o	At both sites, the rain rate and wind speed are lower compared to the other months in between July and September. 
  Both site also see high wind speeds in the first 3 months of the year, but the Offshore site has a smaller rain rate 
  than the Shelf site and then both sites high rain rates in the final couple months of the year, but the Offshore has higher 
  wind speeds than the Shelf site.
•	Which month had the highest rain rate?  Which month had the lowest rain rate?
  o	For the Offshore site, the highest rain rate is in December, and the lowest is in September. 
  o	For the Shelf site, the highest rain rate is in October, and the lowest is in September. 
•	Which month had the highest wind speed? (1 points) Which month had the lowest wind speed?
  o	For the Offshore site, the highest wind speed is in January, and the lowest is in August. 
  o	For the Shelf site, the wind speed is in January, and the lowest is in August. 

Conclusion:

At both sites, the wind speed seems to be the dominating factor between the two parameters. Referencing graphs one and two, 
there is a ton of data points of wind speed covering the plot ranging from zero all the way to 17.5 and they stay consistent 
at 10 m/s throughout the year.
As for the rain rate, there are couple points where the rain is falling hard and getting above 2.5 mm per hour but for the 
most part throughout the year, it is relatively low staying below 0.5 mm/hr. Taking a look at graphs nine and 10, the averages 
for the months are almost all less than 0.1 mm/hr which shows that it is either not raining, or barely at all.
These two observations are even proven in graphs 3 and 4. The plots show that the dominating weather throughout the year is 
Wind and no rain which means it’s not raining a lot and the wind speeds are up.
This conclusion makes sense though since the ocean has high wind speeds majority of the time and it’s not as likely to rain as much.

References:

https://oceanobservatories.org/instrument-series/metbka/

