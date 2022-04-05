## AirBnB Data Analysis Using Google Cloud Platform

Airbnb is one of the most used methods to find a place to stay in most of the major cities in the world. It has dramatically changed the traditional way to find accommodations for short periods of stays and even longer ones. I would mainly like to concentrate on the following questions being raised: 
 * What is the seasonal pattern of Airbnb in Seattle? 
 * What kinds of Airbnb homes are popular? 
 * Prediction of the price. 

The outcome of this project would help businesses narrow down their target marketing customer base towards the most likely prospective customers and this project would also help the business to understand how various attributes affect the client to accept or reject the Airbnb home. 

### Proposed Architecture
![IMG_6E44A272303C-1](https://user-images.githubusercontent.com/30744874/161822507-e50ccab5-ce94-4dea-b7bd-668a68ad9430.jpeg)


### Dataset Description

The data that I would like to use for this project is from http://insideairbnb.com/get-the-data.html .From this I would like to use the following csv data sets. 
  *	Calendar.csv
  *	Listings.csv
  *	Reviews.csv 


### Cleaning of Data set

First we drop the columns with null entries and columns which are almost the same. There are multiple columns for property location, including an attempt by the site that originally scraped the data to clean up the neighbourhood locations. Some of those columns are dropped. Because all listings are in Seattle, columns relating to city and country can be dropped. There are multiple columns for maximum and minimum night stays, but the two main ones will be used as there are few differences between e.g. minimum_nights and minimum_minimum_nights. Several columns only contain one category and are dropped.

### Preliminary EDA

To get the variations of the seasonal rental price we find the mean of the data. To get better patterns we used median and plotted the graphs. For getting the popular home, we did groupby to the listing ids and created a new column called occupancy. Based on the occupancy of the homes and predetermined threshold value we determine which homes are popular and unpopular. Various graphs have been plotted to show the popular and unpopular homes in the considered region.

### Noteworthy findings
By doing the EDA, we find the following
  * Different seasonal patterns in Seattle.
  * Variations of the seasons affecting the bookings.
  * Determined the popular and unpopular homes.
  * Determined the seasonal rental prices.


