---
layout: post
title: Historical collaborative geocoding
subtitle: What is historical geocoding, and how to help historians perform it
tags: [research, publications]
category: research
bigimg: /img/historical_geocoding_abstract.png
---
![geocoding abstract](/img/historical_geocoding_abstract.png)
My recent Postdoctoral position was in the GeoHistorical Data team, for the project Belle Epoque.
The goal is to perform geocoding of historical addresses (aka given an input address and date, find the position on the map).
The projetc heavily relies on extracting information from historical map, and use of database tricks (inheritance, indexes) to robustly and quickly find the geohistorical object that matches the input address and date.
Among the difficulties, everything is fuzzy for geohistorical data : the date of course, but also the spatial position, and even the historical name (misspelling, errors, etc.).

The project led to the developpement of a prototype web GUI (js, based on Leaflet) for collaborative editing.

## Abstract
![historical geocoding abstract](/img/re/historical_geocoding_abstract.png)

The latest developments in digital have provided large data sets that can increasingly easily be accessed and used. These data sets often contain indirect localisation information, such as historical addresses. Historical geocoding is the process of transforming the indirect localisation information to direct localisation that can be placed on a map, which enables spatial analysis and cross-referencing. Many efficient geocoders exist for current addresses, but they do not deal with the temporal aspect and are based on a strict hierarchy (..., city, street, house number) that is hard or impossible to use with historical data. Indeed historical data are full of uncertainties (temporal aspect, semantic aspect, spatial precision, confidence in historical source, ...) that can not be resolved, as there is no way to go back in time to check. We propose an open source, open data, extensible solution for geocoding that is based on the building of gazetteers composed of geohistorical objects extracted from historical topographical maps. Once the gazetteers are available, geocoding an historical address is a matter of finding the geohistorical object in the gazetteers that is the best match to the historical address. The matching criteriae are customisable and include several dimensions (fuzzy semantic, fuzzy temporal, scale, spatial precision ...). As the goal is to facilitate historical work, we also propose web-based user interfaces that help geocode (one address or batch mode) and display over current or historical topographical maps, so that they can be checked and collaboratively edited. The system is tested on Paris city for the 19-20th centuries, shows high returns rate and is fast enough to be used interactively. 

 
## Download link
The article is very much work in progress, 
an [early version is available on arxiv](https://arxiv.org/abs/1703.07138)