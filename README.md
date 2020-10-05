# Citi Bike - Demand Prediction of Bicycles in New York City

This analysis is based upon Citi Bike's dataset of bicycle usage in the city of New York, USA. The purpose of this analysis is to understand the variables available in the dataset, and then determine the factors that would help in predicting the number of bicycles that would required to be stocked outside NyC subway stations. 

The following analysis has been performed:

1. Number of Trips and average duration of trips per bicycles

2. For "Subscribers", trips shorter than 45 minutes are free, and trips over 45 minutes incur a fee. For "Customers", trips shorter than 30 minutes are free, and trips over 30 minutes incur a fee. For each station calculated the proportion of trips started at that station that were free.

3. For each station, we define the station's "drop off popularity" as the number of times a bike was dropped off at that station in our data. For each station, we define the station's "proxy popularity" by looking at all the trips originating from that station, and averaging the drop off popularity of the stations these trips were ended at. For example, suppose station X had three trips in our data; one trip ending at station A (drop off popularity 1500), one ending at station B (drop off popularity 1200), and one ending at station C (drop off popularity 1600), then the proxy popularity for station X is (1500 + 1200 + 1600)/3 = 1433.33. Calculated for each station its proxy popularity.

4. Fit a linear regression model to predict the number of bikes that will be picked up from a station in a given hour based on the hour of day, day of week, and the number of bikes that were picked up from that station in the previous hour.

-
Vishakha Bhattacharjee
MS in Business Analytics, Columbia University
