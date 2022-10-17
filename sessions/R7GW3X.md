---
layout: session
title: "Analyzing changes in OSM over time - full history access to OSM data through the ohsome framework"
code: "R7GW3X"
speaker_names: ['Benjamin Herfort', 'Rafael Troilo']
affiliations: None
room: "Workshops and Loop-Cinema - Room 103"
length: "60"
time: "Saturday, 16:30"
time_iso: "2022-08-20T14:30:00Z"
resources: []
recording: False
---

What is the state of the map in 2022 and how did we get here? Everyone who has used and contributed to OSM knows that the map is constantly evolving: new objects are added, existing data is adjusted and eventually gets deleted. In this workshop we want to explain and show hands-on how you can analyze mapping activity over time through the ohsome framework and how you can interpret the changes, e.g. in respect to data quality, and by combining the ohsome approach with other tools.

<hr>

The OSHDB and ohsome framework have been introduced to the wider OSM community at State of the Map 2018 in Milan. Back then the first version of OSHDB has been released as open-source on GitHub. Here we want to give an update what has happened since then when it comes to uncovering the spatial-temporal dynamics of OSM mapping. Although other software tools like overpass(query language), iOSMAnalyzer(reports), osm2pgsql(database), osm2orc(amazon service) address this problem partially, none of them is able to provide the following range of functionality in one single integrated tool: easy reconstruction of historic geometric and semantic states of the data as well as spatial, temporal and tag queries.

We want to provide an introduction how the ohsome stack (ohsome API, ohsome-dashboard, ohsomeHex, qgis/r/python-plugin, oshdb) can be used for such questions. Based on practical examples and hands-on exercises we've collected over the past years we want to enable the participants to understand the practical usage and enable them to run their own analyses. In this workshop we will show the various endpoints of the ohsome API and we will explain how we've used them in the past. Participants will learn how they can filter for OSM data based on tags, OSM data types (node, way, relation), geometry types (e.g. point, linestring, polygon) or changeset ids. As the OSHDB provides the full spatial and temporal access of the underlying OSM data set, from the state of a single point in time (snapshot) or down to the full edit history of single elements, data can even include indirect contributions and lossless geometric access. (So if you are interested in &#34;broken&#34; geometries we can provide these as well. (wink))

We want to prepare 3-4 hands-on examples. For these it would be good if participants can install QGIS in advance of the workshop. Example (1) will provide an easy entry point towards understanding how OSM changes over time. First, we want to explain how you can count the number of OSM objects, e.g. buildings, on a monthly basis for a given region based on the snapshot view. In Example (2) we want to investigate &#34;re-tagging&#34; activities. Re-tagging can be described as the systematic change of tag values, e.g. highway=unclassified to highway=residential. The example will show how we can detect such activities in OSM using the &#34;groupByTag&#34;-feature and will underline the resulting challenges such activities can have on OSM based metrics. Example (3) will focus on the so-called &#34;contributions&#34;. These can be understood as the changes between two version of an OSM object. For instance, through this concept we can investigate how many new objects have been added to OSM. Maybe even more interesting will be the analysis of further contribution types such as &#34;geometry changed&#34;, &#34;tag changed&#34;, &#34;deleted&#34;. Putting all this together can give us a good understanding of how OSM is expanding and maintained.

