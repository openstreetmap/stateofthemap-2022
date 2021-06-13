---
layout: session
title: "Makina Maps"
code: "9R7LZF"
speaker_names_with_affiliations: ['Frédéric Rodrigo']
room: "Track 1 - Talks"
length: "20"
time: "Friday, 20:00"
time_iso: "2021-07-09T20:00:00Z"
resources: []
recording: True
---
The Vector Tile is a mapping solution where the Data Vector Tiles are served separately from the style and only assembled eg. in the web browser.

Makina Maps is new Vector Tile Server build using Docker and based on Imposm, OpenMapTiles, TileServer GL and NGINX. The stack can be easily and quickly set up. The components allow to import OSM data into a Postgres database and server tiles on request. The tile caching is included. Using Imposm the OSM data can be update and the tiles cache invalided.

This stack can be used as tile server for on request query and support fast update after many improvement was done and still in progress to OpenMapTiles. Fist, it requires to speed up the OpenMapTiles data layers query to server pretty quickly new tiles while users browsing the map. Secondly, it need to be able to update the database as fast the OSM diff update are coming and without locking the database.

In complement of building and serving vector tiles, Makina Maps can hosts vector tile styles and is able to build and server raster version of these tiles. There is also the possibilities to server stored tiles from MBTiles like raster or eg. RGB dynamics light hill shading.
