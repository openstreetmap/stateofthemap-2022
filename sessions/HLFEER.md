---
layout: session
title: "Visualizing Gender of Street Names in Brazil"
code: "HLFEER"
speaker_names_with_affiliations: ["Bernardo Loureiro"]
room: "Track 1"
length: "00:20"
time: "Saturday, 20:00"
resources: []
recording: True
---
Using OSM road data and a database of gender popularity for names, I created a map visualization to show gender disparity in street names in Brazil. Streets named after women represent only a small proportion of the streets in Brazil. This proportion is even smaller when we consider the length instead of the number of streets.

In Brazil, streets are typically named after prominent historical figures, including politicians, business people, military, religious figures, artists, and academics, among others. The small representation of women among these reveals who is chosen to be regarded as prominent, and thus commemorated in a street name, and who isn"t. 

Another interesting aspect is that the map allows up to see certain areas and neighborhoods where female street names predominate. Upon quick visual examination, these appear to be usually in neighborhoods at the periphery of large cities. More in-depth research could indicate if there"s a spatial pattern here and if it is related to other social phenomena.

The interactive map was based on the Road Orientations Map by Vladimir Agafonkin. I used Mapbox and mbtiles for the map visualization. To process the source data, I used Geofabrik extracts of OSM data and Postgres / PostGIS scripts.

The interactive map is here https://medidasp.com/projetos/genero-ruas/#12/-23.5617/-46.6469 and the github repo is here https://github.com/bplmp/genero-ruas-mapa
