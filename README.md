# Mapping_Earthquakes
We will be creating interactive maps using GeoJSON data.

## Table of Contents
- [Overview of Project](#OverviewProject)
  * [Background](#Background)
  * [Purpose](#purpose)
- [Resources](#resources)
- [References](#references)


## <a name="OverviewProject"></a>Overview of Project
### <a name="Background"></a>Background
In this project we are creating an interactive world map using **GeoJSON**, the type of JSON file specifically designed to host geographical information.
GeoJSON data can be found in many apps such as Ride sharing, Navigation and Food Delivery services. It is the industry standard for representing simple geographical features and non spatial attributes. Geographical features such as - Points, contain addresses and locations, like latitude and longitude coordinates. LineStrings, contain coordinates for the boundaries of streets, highways, travel routes and ectonic plates. Ploygons, contain cordinates for the boundaries of zip codes, counties, countries, provinces, and tracts of land. 
Non-spatial attributes, is data that is independent of all geomteric considerations and packaged in a heirarchial structure of GeoJSON file. Examples include, elevation, Temperature, Rain accumulation, Hail Size, Tornado/hurricane strength, Magnitude of an earthquake.


### <a name="Purpose"></a>Purpose

The purpose of this project is to visually show the differences between the magnitudes of earthquakes all over the world for the last seven days.

1. Using our knowledge of **JavaScript and the D3.js** library we will traverse and retrieve the coordinates and magnitudes of the earthquakes from the GeoJSON data. 
2. We'll use the **Leaflet library** to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data. 
3. We will add multiple map layers to geographical maps using Leaflet control plugins to add user interface controls.
4. Add a popup marker that, when clicked, will provide the user with the information about the location and the magnitude of the earthquake.
5. The earthquakes are marked with a circle, and the diameter and the color of the cicle reflect the strength of the earthquake. Earthquakes with higher magnitudes will appear larger and darker in color with a legend providing the context to the map data.
6. finally, to illustrate the relationship between the location and the frequency of the seismic activity and tectonic plates , we will add fault lines on the map.

We will retrive data from the following links:

**Data Source:**

* GeoJson file for Tectonic Plates retrieved from GitHub repository: <br>
  https://github.com/fraxen/tectonicplates/tree/master/GeoJSON
* GeoJson file for Earthquakes for the past 7 days retrieved via API call from USGS website:<br> 
  https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson
* GeoJson file for Major Earthquakes (M4.5+) for the past 7 days via API call from USGS website:<br> 
  https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/4.5_week.geojson

We are adding three different **map styles**:
* Street View
* Satellite View
* Dark View

**The final interactive world map looks as below:**

<p align="center"> <img src = "earthquake_challenge/static/worldmap_gif.gif" width ="45%"> </p> 

## <a name="resources"></a> Resources
[1] [Code for Plotting earthquake data](earthquake_Challenge/static/js/challenge_logic.js) <br>
[2] [HTML file for displaying the data](earthquake_challenge/index.html) <br>
[3] Software: 
 * Visual Studio Code 1.64.2 
 * Chrome Developer Tools <br>
[4] Languages:
 * Jva Script
 * HTML and CSS <br>
[5] Libraries:<br>
 * D3
 * Leaflet

## <a name="references"></a> References
[Mapbox Styles](https://docs.mapbox.com/api/maps/styles/)<br>
[Leaflet Documentation](https://leafletjs.com/)<br>
[Mapbox API retrival](https://www.mapbox.com/)

