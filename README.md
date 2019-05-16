# [Lake Michigan Influences](https://github.com/BlakeWallace/Lake_Michigan_Influences)
05/16/2019

The goal of this project is to explore the influences of the presense of Lake Michigan on the weather in the Chicagoland area. See the Wikipedia article on [The Chicago Metropolitan Area](https://en.wikipedia.org/wiki/Chicago_metropolitan_area).  This project goes granular, attempting to compare various weather parameters at two locations in the area, the [Chicago Botanical Gardens and Ohare International Airport](https://github.com/BlakeWallace/Lake_Michigan_Influences/blob/master/Technical_Report/Technical%20Report/photos/garden_ohare.png).  There are two sections to our analysis.  First, significance testing, to determine whether the data indicates any significant differences between the temperatures and precipitation measurements between the two explored locations.  Second, a predictive model is constructed using the other parameters to attempt to predict the absolute difference in the amount of precipitation between the weather towers at Ohare Airport and the Chicago Botanical Gardens.  There are three data sources used during this exploration.  Two of them are primary to the core of the analyses and model construction.  Our metrics used during our model construction were the mean squared error and the coefficient of determination; and, during significance testing, p-scores.  While the construction of a model in the context of 

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