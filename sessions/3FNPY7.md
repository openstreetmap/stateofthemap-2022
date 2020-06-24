---
layout: session
title: "Ranks for Rendering"
subtitle: "Adding Missing Ranking to OSM Data for Rule-based Cartography"
code: "3FNPY7"
speaker_names_with_affiliations: ["Michael Reichert"]
room: "Track 1"
length: "20"
time: "Saturday, 12:15"
time_iso: "2020-07-04T12:15:00Z"
resources: []
recording: True
pad: https://pad.sotm.bitcast.co.za/p/ranks-for-rendering
---
Maps cannot show all information at all scales. A cartographer needs to decided which features should appear at which scale on the map.

OpenStreetMap based web maps are usually products of rule-based cartography, a computer programme selecting features from a data store and rendering them. It needs rules. If all the features of a feature class are of similar importance, the selection is simple. If not, ranks or attributes to be used for ranking are required. Ranks are assigned to roads as values of the `highway=*` tag, rankable attributes are available as `population=*` tags in OpenStreetMap. 
In some cases some features of a feature class are of high importance but many other features of that class are irrelevant at medium or lower scales.

For example, a map on a medium scale cannot show all stations or all airports in a country. Some airports are only used by a few flights per day, others are not even public. Some train stations have dozens of trains per hours while others get served only few times per week or are used by a dozen passengers per week. Important features should appear at country level but irrelevant features should appear at high scales only.

This challenge has not been addressed by map styles used for OpenStreetMap data so far. Authors of map styles circumvent the issue by rendering all features at higher scales only or by selectiong features randomly until enough features are rendered.

The talk will present how to add ranking information to train stations and airports from OpenStreetMap using other OpenStreetMap data and/or external datasets. The ranking is applied in the rendering database. The ranking train station is based on the presence of public transport route relations and has been used for train station rendering of OpenRailwayMap"s infrastructure map style since January 2020.
