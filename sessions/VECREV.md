---
layout: session
title: "maplibre-rs: Cross-platform Map Rendering using Rust"
code: "VECREV"
speaker_names_with_affiliations: ['Max Ammann (MapLibre)']
room: "&#34;Loop Cinema&#34; - A109"
length: "20"
time: "Friday, 17:05"
time_iso: "2022-08-19T17:05:00Z"
resources: []
recording: False
---
Last year I had a lot of spare time and decided to kick-start a project which combines different areas of interest: Rust, 3D rendering, Geo data
This project was adopted recently by the [MapLibre](https://maplibre.org/) project and is now known as [maplibre-rs](https://github.com/maplibre/maplibre-rs).

The [maplibre-rs](https://github.com/maplibre/maplibre-rs) library is a proof of concept which showed me the complexity of mapping solutions. It takes a lot of steps until edits from OpenStreetMap contributors are finally rendered in consumer applications. With this task I want to take listeners on a journey from drawing changes in the OpenStreetMap editor all the way until vectors are uploaded to from memory to GPUs.

Like outlined in the abstract, I want to cover multiple topics:

* Foundations of digital maps (How to determine which data should be loaded? What are vector and raster tiles?)
* Show the technology stack which allows us to design and develop a cross-platform map renderer (Web, Mobile, Desktop)
