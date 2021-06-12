---
layout: session
title: "A new map renderer for OSM? Rasters, vectors, language and internationalization"
code: "JGF9WA"
speaker_names_with_affiliations: ["Brandon Liu"]
room: "Track 1 - Talks"
length: "20"
time: "Sunday, 16:30"
time_iso: "2021-07-11T16:30:00Z"
resources: []
recording: True
---
OSM"s mission is to create a free, global dataset of geodata for diverse applications. A mainstream OSM use case is **web cartography**: the graphical display of geographic features on the standardized browser platform. Cartographers want to make beautiful, labeled, multi-resolution maps; maps need to be loaded progressively for a smooth user experience. 

The web map status quo centers around two distinct approaches. One approach, used by the OSM Carto project, is server-rendered raster map tiles displayed as images in the browser. Another approach is to use a WebGL framework that consumes tiles of vector features. In the first part of this talk, I will investigate the tradeoffs inherent in these approaches with regards to **multilingual text and internationalization**, as these pose limitations for localizing OSM applications to different languages and cultures. 

The second part of this talk will introduce new techniques and libraries for rendering OSM data that are a compromise between the raster and vector map ecosystems. I"ll demonstrate some of these ideas in protomaps.js, a new Canvas2D and Leaflet-based open source map rendering library, with a focus on a specific use case: Han (Chinese) + Latin mixed-script labeling and custom symbology in Taiwan. I will show how the tools can be extended by developers for other locales; my hope is to build a foundation for **universal mapmaking with OSM data.**
