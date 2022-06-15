---
layout: session
title: "OpenStreetMap in the Cloud"
code: "HEHHCH"
speaker_names: ['Sajjad Anwar']
affiliations: Development Seed
room: "Auditorium A - A001"
length: "20"
time: "Saturday, 09:30"
time_iso: "2022-08-20T09:30:00Z"
resources: []
recording: True
---

The geospatial world is moving to cloud-first and cloud-native approaches. Movements like STAC and COG have transformed how people use raster data in the last couple of years. OpenStreetMap has much to gain from thinking about different cloud infrastructure architectures. This talk will discuss what it takes to run the OpenStreetMap ecosystem in the cloud and present the history and work on a project called [OSM Seed](https://github.com/developmentseed/osm-seed/). We learned so much while building OSM Seed and think it can be a blueprint for running OpenStreetMap on cloud infrastructure.

<hr>

The OpenStreetMap ecosystem contains many open source software projects beyond the Rails application. This includes tools that are used by mappers on a daily basis, like, Overpass, Tasking Manager, iD, JOSM, tile servers, data processing applications, Nominatim and so on. It’s a complex ecosystem of growing tools. These are maintained by different individuals and organisations. OSM Seed started in 2018 after several attempts to containerise OSM software for easy installation. [I talked about this vision](https://2015.stateofthemap.us/openstreetmap-software-for-more-than-openstreetmap) in 2015 at State of the Map US. Since then, OSM Seed has grown to be a mature and heavily tested software project that now powers projects like OpenHistoricalMap and data projects at Humanitarian OpenStreetMap Team.

We learned so much while building OSM Seed and think it can be a blueprint for running OpenStreetMap on cloud infrastructure. OSM Seed uses cloud agnostic approaches through Kubernetes to bring together projects that make up what OSM is today. These projects continue to get updates and are maintained how they always have been. OSM Seed provides an interface to bring the ecosystem a little closer through better infrastructure orchestration.

In this talk, I’d like to discuss a brief history of OSM Seed, some of our lessons trying to move OSM software to the cloud, and open a conversation on what could be useful for OSM going forward.

