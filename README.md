# [Lake Michigan Influences](https://github.com/BlakeWallace/Lake_Michigan_Influences)
Creation Date: 05/16/2019
Most Recent Work: 06/04/2025

The goal of this project is to explore the influences of the presense of Lake Michigan on the weather in the Chicagoland area. See the Wikipedia article on [The Chicago Metropolitan Area](https://en.wikipedia.org/wiki/Chicago_metropolitan_area).  The fact of [Lake Effect-snow](https://en.wikipedia.org/wiki/Lake-effect_snow) is well documented.  This project adds to the discussion by considering precipitation and temperature.  

**Contents**

  - [README](https://github.com/BlakeWallace/Lake_Michigan_Influences#lake-michigan-influences) - Provides an overview of the repository  
  - [Research_Process](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/working/Research_Process.md)  
  - [References](https://github.com/BlakeWallace/Lake_Michigan_Influences/tree/master/References)  
      - [Spatio-Temporal_Modelling_In_The_Pacific_NW.pdf](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/References/Spatio-Temporal_Modelling_In_The_Pacific_NW.pdf?raw=true)  
  - [Technical Report](https://github.com/BlakeWallace/Lake_Michigan_Influences/tree/master/Technical_Report)  
      - [photos](https://github.com/BlakeWallace/Lake_Michigan_Influences/tree/master/Technical_Report/Technical%20Report/photos) - photos used in the report  
      - [Technical Report.pdf](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/Technical_Report/Technical%20Report/Technical%20Report.pdf?raw=true)  
      
**Data**  

  - [data](https://github.com/BlakeWallace/Lake_Michigan_Influences/tree/master/data) - Contains various datasets that will be found in the notebooks.  
  
**Jupyter Notebooks**  

  - [1_scraping_great_lakes_daily_average_temp_1995_2018](https://nbviewer.org/github/BlakeWallace/Lake_Michigan_Influences/blob/master/1_scraping_great_lakes_daily_average_temp_1995_2018.ipynb) - Collecting the data for Lake Michigan average daily temperatures  
  - [2_cleaning_lake_michigan_temp_data_1995_2019](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/2_cleaning_lake_michigan_temp_data_1995_2019.ipynb) - Cleaning the lake michigan data.  
  - [3_merging_the_data](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/3_merging_the_data.ipynb) - Cleaning and merging various datasets for analysis.  
  - [4_EDA_and_analysis](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/4_EDA_and_analysis.ipynb) - Exploratory Data Analysis of the data before modeling.  
  - [5_modeling](https://nbviewer.org/github/BlakeWallace/Lake_Michigan_Influences/blob/master/5_modeling.ipynb) - T-testing and predictive modelling.  
 
**Overview**  
  
The National Weather Service monitors a plethora of weather variables utilizing several different techniques, including satelites, buoys, towers, and ballons.  During this project, surface data collected at weather towers and buoys was explored.  The underlying analysis is granular in that it compares various weather parameters at two specific locations in the Chicagoland area, the [Chicago Botanical Gardens and Ohare International Airport](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/Technical_Report/Technical%20Report/photos/garden_ohare.png).   

There are two sections to the analysis.  First, two-tailed t-testing, to determine whether the data indicates any significant differences in temperature and precipitation measurements between the two locations.  Second, predictive modeling.  To this end, a predictive model is constructed using supplemental parameters to attempt to predict the absolute difference in the amount of precipitation between the weather towers at Ohare Airport and the Chicago Botanical Gardens.  

There are three data sources used during this exploration.  Two of them are primary to the core of the analysis and modeling.  The third is planned for future iterations.  The metrics used during model construction are the mean squared error and the coefficient of determination.  During significance testing, p-scores of two-tailed t-tests are analyzed to determine levels of safely excepting differences in temperatures.  

While the construction of a predictive model in the context of our data proved to be less than ideal, the t-testing does clearly show significant temperature differences under various weather conditions.

**Sources:** 
 - Primary
1.  [NOAA National Centers for Environmental Information's Global Historical Climatology Network (GHCN)](https://www.ncdc.noaa.gov/cdo-web/search)
     - [CHICAGO OHARE INTERNATIONAL AIRPORT, IL US](https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USW00094846/detail)
     - [CHICAGO BOTANIC GARDEN, IL US](https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USC00111497/detail)
2.  [Great Lakes Statistics: Average Surface Water Temperature from the Great Lakes Surface Environmental Analysis (GLSEA)](https://coastwatch.glerl.noaa.gov/statistic/statistic.html)
     - [Lake Michigan](https://en.wikipedia.org/wiki/Lake_Michigan)
 - Secndary
3.  [National Data Buoy Center (NDBC)](https://www.ndbc.noaa.gov/)  
     - [Station FSTI2 - Foster Ave., Chicago, IL](https://www.ndbc.noaa.gov/station_page.php?station=fsti2)

**[Data Information](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/data/Data_Dictionaries/Data_Information.md)** 