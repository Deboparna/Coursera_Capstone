# Fast Food Restaurant Analysis in Four Metropolitan Cities in India - Report

## Table of contents:
1. [Introduction: Business Problem](#introduction)
2. [Data Requirements](#data)

## Introduction: Business Problem<a name="introduction"></a>

### The Problem
This project deals with discussing the neighborhoods of the four metropolitian cities of India namely; New Delhi, Mumbai, Kolkata and Chennai. This would specifically help answer some questions regarding the density of fast food restaurants.

The Foursquare API is used to access the top 100 venues in each neighborhood. Next, we map the data using the Folium library to visualise the density of the restaurants in each city. After which we even have find the mean distance between all the restaurants and the mean coordinates of the city. This is the find out which city among the four has the most dense distribution of fast food restaurants.

### Target Audience
The major target audience could either be health researchers trying to find corelation between fast food and various health problems. Or another audience could be the people trying to find an ideal city to start fast food business in. Perhaps a city with relatively less density might mean less competetion for these people?

### Pressing Questions
* Which city would give most and least competetion while starting a fast food restaurant?
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
