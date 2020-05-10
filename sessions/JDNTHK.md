---
layout: session
title: "Minutely Extracts: Tools for nimble editing and downloading"
code: "JDNTHK"
speaker_names_with_affiliations: ["Brandon Liu"]
room: "Track 1"
length: "00:20"
time: "Sunday, 17:15"
time_iso: "2020-07-05T17:15:00Z"
resources: []
recording: True
---
Workflows for adding data to OpenStreetMap keep getting better - but once an edit is uploaded, it can take a long time to appear on hosted map tiles or regional OSM extracts. The experience of downloading and using OpenStreetMap can be improved by quick access to fresh data - a fast feedback loop makes contributing to OSM more enjoyable!

The first part of this talk covers a new web service, Minutely Extracts (protomaps.com/extracts). Mappers can download rectangular or polygon regions of the world, with changes replicated every minute from planet.openstreetmap.org. I’ll show some example workflows for using Minutely Extracts with common GIS applications such as QGIS, and new tools for conversion to formats like GeoPackage and Shapefile.

The second part of this talk describes OSM Express (osmx), a new spatially indexed file format powering Minutely Extracts, that supports in-place updates. Developers needing random access to OSM objects can consider embedding osmx as a library. Near real-time editing activity visualization is one possible use case. I’ll review the technical tradeoffs between using osmx, PBFs and other popular formats.

Financial Background: The software is developed as open source, under a BSD license, and funded by the author"s commercial OSM-based SaaS services as well as OSM contract software development.
