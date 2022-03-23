# PyBer_Analysis_Challenge

## Overview 
The manager at PyBer ride sharing company has given us a brand-new assignment to use our Python skills and knowledge of Pandas to create a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, create a multiple-line graph that shows the total weekly fares for each city type. Finally, submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer.


## Procedures & Results:

We started by converting the city data csv file and ride data csv files into Pandas Dataframes. We instected the data for any null values. Then we used the Pandas unique() function to find the types of cities in our city data.  There are three city types: Urban, Suburban, and Rural.   Then we merged both DataFrames to do our analysis.  Later, we created separate Dataframes for each city to analyze riding trends and calcuations. Below is an example of total number of rides in Urban city:

![Screen Shot 2022-03-23 at 11 25 13 AM](https://user-images.githubusercontent.com/98566486/159734993-d466757a-0988-4b47-90c4-e5a6cb022547.png)

Our analysis shows the following results.

#### The total number of rides per city:

* Urban : 1625
* Suburban: 625
* Rural: 125

#### The total number of rides per city:

* Urban : 1625
* Suburban: 625
* Rural: 125


#### The total number of drivers per city:

* Urban : 2405
* Suburban: 490
* Rural: 78

#### The total fares per city:

* Urban : $39,854.38
* Suburban: $19,356.33
* Rural: $4327.93


 #### The average fare per ride per city:
 
* Urban : $24.53
* Suburban: $30.97
* Rural: $34.62

#### The average fare per driver per city:
 
* Urban : $16.57
* Suburban: $39.50
* Rural: $55.49

These analysis can be seen through our summary dataframe:

![Screen Shot 2022-03-23 at 11 53 31 AM](https://user-images.githubusercontent.com/98566486/159741261-cee500eb-5845-4000-8c57-569a61825e54.png)

We further enhance the analysis by creating a multiple line plot to show the total weekly fares for each type of city by creating new dataframe for the total fare by date and we used the groupby() function to aggregate the calculations.  

![Screen Shot 2022-03-23 at 11 57 17 AM](https://user-images.githubusercontent.com/98566486/159742078-21089053-9cfb-4cbb-8a30-181bfb771206.png)

Then we created a pivot table with the dates as the index to get the total fares for each type of city by the date. We found the weekly total sum for fares for each city for the first quarter of the year.

![Screen Shot 2022-03-23 at 12 01 04 PM](https://user-images.githubusercontent.com/98566486/159742868-53ba8dac-596b-4d37-b56c-8158b93298c9.png)

Finally, we imported style from the matplotlib to style our multiline plot.  

![Screen Shot 2022-03-23 at 12 02 55 PM](https://user-images.githubusercontent.com/98566486/159743235-6937c5ec-d114-40be-9aa0-944aed9ba425.png)

## Summary:


Ride Summary based on the Pyber Rides Summary data appears to reflect what probably most people would expect. Total Rides: Urban areas have approximately 3x as many rides as Suburban areas which in turn have approximately 4x as many rides as rural areas. Total Drivers: Urban areas have many more drivers. Total Fares show expected breakdowns, but not by the same factors as Total Rides. Average per Ride Fare reflects Rural areas generating approximately $4 more per ride that Suburban which in turn generating approximately $6 more than Urban. This may be accounted for by longer distances in Rural areas costing more per ride. Rural city Average per Driver dominated almost 3x the rate of Urban.  

Our three suggestions to the PyBer Bussiness decision makers are as follow:

* It seems like the Rural cities are underserved, but it needs further research and analysis for rural cities to justify the need before making an investment to improve total rides and drivers count.  Customers are paying higher fares in Rural cities.
* Drivers in Urban cities are generating way less income compared to Suburban and Rural Cities.  However, PyBer is generating the most revenue in Urban cities.  There should be review for making drivers' income better throughout the Urban cities.
* The first quarter analysis is not enough to make any major decision.  It would be a good idea to run the yearly analysis to further enhance the results before making any improvement investment such as hiring more drivers or adjusting the ride fares.




