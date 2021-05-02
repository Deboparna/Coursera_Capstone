# Fast Food Restaurant Analysis in Four Metropolitan Cities in India - Report

## Table of contents:
1. [Introduction: Business Problem](#introduction)
2. [Data](#data)
3. [Methodology](#methodology)
4. [Analysis](#analysis)
5. [Result](#results)
6. [Discussion](#discussion)
7. [Conclusion](#conclusion)

## Introduction: Business Problem<a name="introduction"></a>

### The Problem
This project deals with discussing the neighborhoods of the four metropolitan cities of India namely; New Delhi, Mumbai, Kolkata and Chennai. This would specifically help answer some questions regarding the density of fast food restaurants.

The Foursquare API is used to access the top 100 venues in each neighborhood. Next, we map the data using the Folium library to visualize the density of the restaurants in each city. After which we even have find the mean distance between all the restaurants and the mean coordinates of the city. This is the find out which city among the four has the most dense distribution of fast food restaurants.

### Target Audience
The major target audience could either be health researchers trying to find correlation between fast food and various health problems. Or another audience could be the people trying to find an ideal city to start fast food business in. Perhaps a city with relatively less density might mean less competition for these people?

### Pressing Questions
* Which city would give most and least competition while starting a fast food restaurant?
* Do health problems like obesity have anything to do with the ever increasing fast food restaurants?

## Data<a name="data"></a>

In order to obtain the venue details in each city Foursquare API is used.

https://foursquare.com/

The following data are obtained from the Foursquare API:
1. Venue Name
2. Venue Address
3. Venue Latitude
4. Venue Longitude

A total of 300 venues data have been obtained from Foursquare.

## Methodology<a name="methodology"></a>

We gathered the neighborhood data of all the metropolitan city by category ID. We also have the top 100 in each city obtained using Foursquare API. A total of 300 venues have been obtained in all the cities of fast food category.

We have first plotted all these restaurant locations on a map and tried to get a visual idea of how these restaurants are spread over. We also got the total count of fast food restaurant per city. This gave us an idea of which city has the most number of fast food restaurants.

We followed this path of study and further tried to understand the density of these restaurants in each city. We have done so by calculating the mean distance from all these restaurants to the mean coordinate of the respective city. After find out the mean distance we tried to visualize this on the map. This gave us a better idea about the fast food restaurants throughout each city as we incorporated the distance factor into it.

## Analysis<a name="analysis"></a>
### Exploring Fast Food Places
On searching for fast good restaurants in the 4 cities we found this result:

* Total number of fast food places in New Delhi = 94
* Total number of fast food places in Kolkata = 25
* Total number of fast food places in Mumbai = 117
* Total number of fast food places in Chennai = 64

Mapping the locations of all 300 fast food restaurants in 4 cities:

### Mumbai
![Mumbai Map](https://github.com/Deboparna/Coursera_Capstone/blob/main/Week%204/images/mumbai.png)
### Kolkata
![Mumbai Map](https://github.com/Deboparna/Coursera_Capstone/blob/main/Week%204/images/kolkata.png)
### Chennai
![Mumbai Map](https://github.com/Deboparna/Coursera_Capstone/blob/main/Week%204/images/chennai.png)
### New Delhi
![Mumbai Map](https://github.com/Deboparna/Coursera_Capstone/blob/main/Week%204/images/new-delhi.png)

### Looking at the density of these restuarants.
We then proceeded to calculate the mean distance from from mean coordinates of the restaurant of the respective city. On calculation we found:

* Mean Distance from Mean coordinates of New Delhi: 0.0812
* Mean Distance from Mean coordinates of Kolkata: 0.0551
* Mean Distance from Mean coordinates of Mumbai: 0.07124
* Mean Distance from Mean coordinates of Chennai: 0.04487

Mapping the locations of all 300 fast food restaurants in 4 cities with mean distance:
### Mumbai
![Mumbai Map](https://github.com/Deboparna/Coursera_Capstone/blob/main/Week%204/images/mumbai-dist.png)
### Kolkata
![Mumbai Map](https://github.com/Deboparna/Coursera_Capstone/blob/main/Week%204/images/kolkata-dist.png)
### Chennai
![Mumbai Map](https://github.com/Deboparna/Coursera_Capstone/blob/main/Week%204/images/chennai-dist.png)
### New Delhi
![Mumbai Map](https://github.com/Deboparna/Coursera_Capstone/blob/main/Week%204/images/new-delhi-dist.png)

## Results<a name="results"></a>
* Looking into the total fast food restaurant number we can confidently say that Mumbai is the city with the highest number of such restaurants and Kolkata the least.
* In the second half we can conclude that although Mumbai has the highest fast food restaurants, it is Chennai with the least mean distance. In short, the density of these restaurants is the highest in Chennai. While New Delhi proved to be the most sparse.

## Discussion<a name="discussion"></a>
Now to answer our pressing questions,

* Which city would give most and least competition while starting a fast food restaurant?
New Delhi would prove to be the best location to open new fast food restaurants considering its low density. This would mean low competition for the newcomer and along with good business ethics the business would be blooming in no time.

* Do health problems like obesity have anything to do with the ever increasing fast food restaurants?
In terms of obesity rates; the city with the highest percent of overweight population is Mumbai, shortly followed by Kolkata and Chennai [[Source](https://www.statista.com/statistics/1119418/india-body-mass-index-by-select-city/ "Source")]. This might be related to the high number of fast food restaurants in Mumbai however correlation does not always imply causation. Hence, with just this amount of data it is impossible to come to any conclusion.

## Conclusion<a name="conclusion"></a>
Purpose of this project was to analyze the four metropolitan cities of India and analyze fast food restaurants within them. The neighborhoods data was obtained from the Foursquare API was used to find the major venues in each city. We mapped the data found and with its help, tried to draw results from the venue distribution and were able to point out a few useful observations.
