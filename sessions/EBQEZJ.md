---
layout: session
title: "Building a global outdoor map"
code: "EBQEZJ"
speaker_names_with_affiliations: ["Jiri Komarek"]
room: "Track 1 - Talks"
length: "20"
time: "Sunday, 20:00"
time_iso: "2021-07-11T20:00:00Z"
resources: []
recording: True
---
MapTiler Outdoor is a global dataset and a map style for hiking and biking available as a zoomable and web-compatible vector tiles, which are ready for use in OpenLayers, MapLibre, Leaflet, QGIS as well as mobile applications.

After first excitement, challenges starts to appear one after another: most of them originating from a need to create a rigid set of rules for the entire world, which is full of diversity due to the variety of nature. We also faced the challenge of lacking international standardization for hiking trails, which is unique for each country (and even on this level with many exceptions and specialities - like oneways, via ferrata routes or even climbing trails). And last, but not least, we have to dig all this information from the OpenStreetMap and turn it into a map understandable for everyone. 

We managed to create a layer with trails and corresponding points of interest, which can be filtered on hiking or biking in the customize tool. This layer can be overlaid on top of any map. However, we created a specialized map style which combines OpenStreetMap with contour lines and hillshade and highlights things you need for moving around in the nature. 

The schema of MapTiler Outdoor is based on the open-source OpenMapTiles (OTM) schema and data are processed using OMT stack.

MapTiler Outdoor is available via MapTiler Cloud as a service or in a form of a data package for download.
