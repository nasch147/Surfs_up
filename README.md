# Surfs_up

## Overview
The purpose of the analysis is to evaluate the suitability of weather patterns in Oahu, HI for the opening of a surf supply and ice cream business. Specifically, this analysis focused on patterns for the months of June and December to see if business activity, as dictated by the weather, would be viable year-round. 

Our data consisted of precipitation and temperature readings from 9 weather measurement stations from 2010 to 2017 near our selected site.  The readings data was stored in a SQLite database. The SQLAlchemy was used via jupyter notebook to query and map the data and allowing us to do so through python. the data was then added to a dataFrame and analyzed using the pandas library. Because we are only examining the months of June and December, the data was filtered by extracting the date from the data using SQLAlchemy. 

## Results

### Statistical Summary
![JUN](Resources/June_Data_Summary.png)
![DEC](Resources/December_Data_Summary.png)

### Key Findings

- **As would be expected, temperatures in June are generally higher than those in December** 
  -  The average temperature in June is approximately 5.6% higher than that of December. Also, minimum, maximum, and percentile temperatures are also all higher for the month of June. 
- **There is more volatility inherent in the December temperatures**
  - the standard deviation of temperatures in December was 3.75 degrees versus 3.25 in June. Higher levels of volatility in temperature indicates increased business risk during the winter months. 
- **The relative uniformity in temperatures throughout the year make the site much more attractive than most places in the world**
  - Although there is increased volatility and generally lower temperatures in December, the temperature data indicates that weather in Oahu is much more supportive of a year-round surf and ice cream business as compared to most other places in the world.  Indeed with only a 5.6% difference in winter and summer temperatures combined with a relatively low standard deviation in temperatures, it makes the site ideal as compared to locations further form the equator. 

## Summary
Overall, the site on Oahu for a surf and ice cream shop is ideal to conduct business year-round when examining temperature and precipitation data. There is relatively low volatility of temperatures throughout the year and winter temperatures are sufficiently high to continue to support ice cream sales. However, it is recommended that the following two additional data points be measured to effectively evaluate the site selection:
- Surf and Tide trends should collected and analyzed to understand the site from the perspective of the surf rental business. Data from NOAA should be accessed via API in order to conduct this analysis
- Tourism flows should also be examined throughout the year to better be able to plan for high-and-low seasonality. Data regarding this factor might be found through the department of tourism for Hawaii or GDP data can be gathered through the Bureau of Economic Analysis for the hospitality sector. 
