# [Lake Michigan Influences](https://github.com/BlakeWallace/Lake_Michigan_Influences)
05/16/2019

The goal of this project is to explore the influences of the presense of Lake Michigan on the weather in the Chicagoland area. See the Wikipedia article on [The Chicago Metropolitan Area](https://en.wikipedia.org/wiki/Chicago_metropolitan_area).  The fact of [Lake Effect-snow](https://en.wikipedia.org/wiki/Lake-effect_snow) is well documented.  This project adds to the discussion by considering precipitation and temperature.  

**Contents**

  - [README](https://github.com/BlakeWallace/Lake_Michigan_Influences#lake-michigan-influences) - Provides an overview of the repository  
  - [Technical Report](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/Technical_Report/Technical%20Report/Technical%20Report.pdf)  
 **Data**
  - [data](https://github.com/BlakeWallace/Lake_Michigan_Influences/tree/master/data) - Contains various datasets that will be found in the notebooks.  
 **Jupyter Notebooks**
  - [1_scraping_great_lakes_daily_average_temp_1995_2018](https://render.githubusercontent.com/view/ipynb?commit=7659dcac22b66767ebc65f487be42f653121e4cc&enc_url=68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f426c616b6557616c6c6163652f4c616b655f4d6963686967616e5f496e666c75656e6365732f373635396463616332326236363736376562633635663438376265343266363533313231653463632f315f7363726170696e675f67726561745f6c616b65735f6461696c795f617665726167655f74656d705f313939355f323031392e6970796e62&nwo=BlakeWallace%2FLake_Michigan_Influences&path=1_scraping_great_lakes_daily_average_temp_1995_2018.ipynb&repository_id=183659877&repository_type=Repository#In-this-notebook-we-work-through-the-code-needed-to-scrape-the-Average-Daily-Water-temperatures-for-the-great-lakes-from-the-National-Weather-Service's-website) - Collecting the data for Lake Michigan average daily temperatures  
  - [2_cleaning_lake_michigan_temp_data_1995_2019](https://render.githubusercontent.com/view/ipynb?commit=7659dcac22b66767ebc65f487be42f653121e4cc&enc_url=68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f426c616b6557616c6c6163652f4c616b655f4d6963686967616e5f496e666c75656e6365732f373635396463616332326236363736376562633635663438376265343266363533313231653463632f325f636c65616e696e675f6c616b655f6d6963686967616e5f74656d705f646174615f313939355f323031392e6970796e62&nwo=BlakeWallace%2FLake_Michigan_Influences&path=2_cleaning_lake_michigan_temp_data_1995_2019.ipynb&repository_id=183659877&repository_type=Repository#Cleaning-the-water-temperature-data-for-Lake-Michigan) - Cleaning the lake michigan data.  
  - [3_merging_the_data](https://render.githubusercontent.com/view/ipynb?commit=7659dcac22b66767ebc65f487be42f653121e4cc&enc_url=68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f426c616b6557616c6c6163652f4c616b655f4d6963686967616e5f496e666c75656e6365732f373635396463616332326236363736376562633635663438376265343266363533313231653463632f335f6d657267696e675f7468655f646174612e6970796e62&nwo=BlakeWallace%2FLake_Michigan_Influences&path=3_merging_the_data.ipynb&repository_id=183659877&repository_type=Repository#Merging-data) - Cleaning and merging various datasets for analysis.  
  - [4_EDA_and_analysis](https://render.githubusercontent.com/view/ipynb?commit=31b9c230c98e47d9646d7128b60e8478a52ee21a&enc_url=68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f426c616b6557616c6c6163652f4c616b655f4d6963686967616e5f496e666c75656e6365732f333162396332333063393865343764393634366437313238623630653834373861353265653231612f345f4544415f616e645f616e616c797369732e6970796e62&nwo=BlakeWallace%2FLake_Michigan_Influences&path=4_EDA_and_analysis.ipynb&repository_id=183659877&repository_type=Repository#Analysis-of-the-data) - Exploratory Data Analysis of the data before modeling.  
  - [5_modeling](https://render.githubusercontent.com/view/ipynb?commit=7659dcac22b66767ebc65f487be42f653121e4cc&enc_url=68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f426c616b6557616c6c6163652f4c616b655f4d6963686967616e5f496e666c75656e6365732f373635396463616332326236363736376562633635663438376265343266363533313231653463632f355f6d6f64656c696e672e6970796e62&nwo=BlakeWallace%2FLake_Michigan_Influences&path=5_modeling.ipynb&repository_id=183659877&repository_type=Repository#Modeling-the-Garden-Ohare-Lake-Michigan-data-(1995-2018)) - T-testing and predictive modelling.  
 
**Overview**  
  
The National Weather Service monitors a plethora of weather variables utilizing several different techniques, including satelites, buoys, towers, and ballons.  During this project, surface data collected at weather towers and buoys was explored.  The underlying analysis is granular in that it compares various weather parameters at two specific locations in the Chicagoland area, the [Chicago Botanical Gardens and Ohare International Airport](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/Technical_Report/Technical%20Report/photos/garden_ohare.png).   

There are two sections to the analysis.  First, two-tailed t-testing, to determine whether the data indicates any significant differences in temperature and precipitation measurements between the two locations.  Second, as a data scientist. the goal is to use data to make predictions.  To this end, a predictive model is constructed using supplemental parameters to attempt to predict the absolute difference in the amount of precipitation between the weather towers at Ohare Airport and the Chicago Botanical Gardens.  

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

**[Data Information](https://render.githubusercontent.com/view/ipynb?commit=81f218ce41e7bc575aa19aa3d07b72a2a92272fb&enc_url=68747470733a2f2f7261772e67697468756275736572636f6e74656e742e636f6d2f426c616b6557616c6c6163652f4c616b655f4d6963686967616e5f496e666c75656e6365732f383166323138636534316537626335373561613139616133643037623732613261393232373266622f646174612f446174615f44696374696f6e61726965732f446174615f496e666f726d6174696f6e2e6970796e62&nwo=BlakeWallace%2FLake_Michigan_Influences&path=data%2FData_Dictionaries%2FData_Information.ipynb&repository_id=183659877&repository_type=Repository#Data-Information)** 