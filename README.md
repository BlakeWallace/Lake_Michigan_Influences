# [Lake Michigan Influences](https://github.com/BlakeWallace/Lake_Michigan_Influences)
05/16/2019

The goal of this project is to explore the influences of the presense of Lake Michigan on the weather in the Chicagoland area. See the Wikipedia article on [The Chicago Metropolitan Area](https://en.wikipedia.org/wiki/Chicago_metropolitan_area).  There are two things....There are three data sources used during this exploration.  Two of them are primary to the core of the analyses and model construction.  Our metrics used during our model construction were the mean squared error and the coefficient of determination.  The construction of a model in the context of 

**Sources:** 
 - Primary
1.  [Global Historical Climatology Network (GHCN) – Daily Documentation](https://www1.ncdc.noaa.gov/pub/data/cdo/documentation/GHCND_documentation.pdf)
2.  [Great Lakes Statistics: Average Surface Water Temperature from the Great Lakes Surface Environmental Analysis (GLSEA)](https://coastwatch.glerl.noaa.gov/statistic/statistic.html)
 - Secndary
3.  [National Data Buoy Center (NDBC)](https://www.ndbc.noaa.gov/)  

**Data:**
#### [CHICAGO OHARE INTERNATIONAL AIRPORT, IL US](https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USW00094846/detail)
 - Source: [National Centers for Environmental Information](https://www.ncdc.noaa.gov/cdo-web/search)  
 - [GHCN (Global Historical Climatology Network) – Daily Documentation](https://www1.ncdc.noaa.gov/pub/data/cdo/documentation/GHCND_documentation.pdf)
  - ID	GHCND:USW00094846  
    41.995 N 87.9336 W 
 - [Airport Information](https://www.flychicago.com/ohare/home/pages/default.aspx)
 
#### [CHICAGO BOTANIC GARDEN, IL US](https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USC00111497/detail)
 - Source: [National Centers for Environmental Information](https://www.ncdc.noaa.gov/cdo-web/search)
 - [GHCN (Global Historical Climatology Network) – Daily Documentation](https://www1.ncdc.noaa.gov/pub/data/cdo/documentation/GHCND_documentation.pdf)
  - ID GHCND:USC00111497
    42.13987 N 87.78537 W
 - [Garden Information](https://www.chicagobotanic.org/?gclid=CjwKCAjw8e7mBRBsEiwAPVxxiFAzbi0I4VKZUO1z3uxcDI36xORzYwbOtmUWGVoUqxRHEi8elJFV2RoCmaoQAvD_BwE)
    
#### [Lake Michigan](https://www.google.com/search?q=lake+michigan&oq=lake+michigan&aqs=chrome.0.69i59j69i60l3j69i59j0.3015j0j9&sourceid=chrome&ie=UTF-8)
 - Source: [Great Lakes Statistics: Average Surface Water Temperature from the Great Lakes Surface Environmental Analysis (GLSEA)](https://coastwatch.glerl.noaa.gov/statistic/statistic.html)
 - 44.0 -87.0 (44° 00' 0.00" N 87° 00' 0.00" W)
 - [Example Data Set from 2018](https://coastwatch.glerl.noaa.gov/ftp/glsea/avgtemps/2018/glsea-temps2018_1024.dat)
 
#### [Station FSTI2 - Foster Ave., Chicago, IL](https://www.ndbc.noaa.gov/station_page.php?station=fsti2)
 - Source: [National Data Buoy Center](https://www.ndbc.noaa.gov/)

 - Owned and maintained by [Chicago Park District](https://www.ndbc.noaa.gov/ndbcexit.php?url=https://wqdatalive.com/public/16&blurb=Chicago+Park+District)  
    41.976 N 87.648 W (41°58'35" N 87°38'51" W)


1.  An executive summary:
What is your goal?
Where did you get your data?
What are your metrics?
What were your findings?
What risks/limitations/assumptions affect these findings?
2. Summarize your statistical analysis, including:
implementation
evaluation
inference
3. Clearly document and label each section of your notebook(s)
Logically organize your information in a persuasive, informative manner.
Include notebook headers and subheaders, as well as clearly formatted markdown for all written components.
Include graphs/plots/visualizations with clear labels.
Comment and explain the purpose of each major section/subsection of your code.
Document your code for your future self, as if another person needed to replicate your approach.
4. Clearly document all of your decision points in the relevant sections
How did you acquire your data?
How did you transform or engineer your data? Why?
How did you select your model?
How did you optimize hyperparameters?
5. Host your notebook and any other materials in your own public Github Repository.
You repo should have README file that guides us through the repository and links to important files.
Include links and explanations to any outside libraries or source code used.
Host a copy of your dataset or include a link to a remotely hosted version.