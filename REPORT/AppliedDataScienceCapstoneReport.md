# Applied Data Science Capstone Project Report

## Introduction/Business Problem

Kyoto is one of the oldest city in Japan and there are quite a lot of historical structures. It attracts many foreign tourists every year.

If someone is looking to open a travel agency with local guide service for the tourists, where would be recommended that they setup their office?

## Data

We use the following 4 data for analysis.

### Japan postal code

First of all, we need address data of Kyoto city.
We use [postal code data](https://www.post.japanpost.jp/zipcode/dl/roman/ken_all_rome.zip?190712) distributed from Japan Post Corporation.

The postal code data is in CSV format with the following columns.

1. zip code
2. prefecture (Japanese)
3. borough (Japanese)
4. neighborhood (Japanese)
5. prefecture (English)
6. borough (English)
7. neighborhood (English)

### [geopy](https://geopy.readthedocs.io/)

The postal code data does not have coordinates. So we use [geopy](https://geopy.readthedocs.io/) library to look up them from `prefecture (Japanese)`, `borough (Japanese)`, and `neighborhood (Japanese)` in the postal code data.

### [Folium location data](https://python-visualization.github.io/folium/)

After getting the coordinates of each neighborhood, we use [Folium location data](https://python-visualization.github.io/folium/) to plot them and explore locations on map.

### [Foursquare API](https://api.foursquare.com)

To get the characteristics of neighborhoods, we use [Foursquare API](https://api.foursquare.com) to see venues information near by them.

## Methodology

## Results

## Discussion

## Conclusion
