---
layout: session
title: "maplibre-rs: Cross-platform Map Rendering using Rust"
code: "VECREV"
speaker_names: ['Max Ammann']
affiliations: MapLibre
room: "Workshops/&#34;Loop Cinema&#34; - Room 103"
length: "20"
time: "Friday, 16:30"
time_iso: "2022-08-19T14:30:00Z"
resources: [{ description: "slides", url: "/attachments/VECREV_2022-08-19-SotM-maplibre-rs_sO0aXrv.pdf" }]
recording: False
---

Digital maps are ubiquitous tools in our everyday life. In the early 90s, the idea of browsing the world digitally and visiting any place was groundbreaking. The first solution to this problem is known as &#34;TerraVision&#34;, which was breathtaking. Today, the idea of exploring your surroundings using digital maps has become normal.

But how do these maps work? In this talk, I want to provide an overview of the foundations of digital mapping solutions. Differences between maps which use vector data and rasterized satellite imaginary will be outlined. Furthermore, a new and open-source map renderer called maplibre-rs will be presented, which is created using Rust and WebGPU.

<hr>

Last year I had a lot of spare time and decided to kick-start a project which combines different areas of interest: Rust, 3D rendering, Geo data
This project was adopted recently by the [MapLibre](https://maplibre.org/) project and is now known as [maplibre-rs](https://github.com/maplibre/maplibre-rs).

The maplibre-rs library is a proof of concept which showed me the complexity of mapping solutions. It takes a lot of steps until edits from OpenStreetMap contributors are finally rendered in consumer applications. With this task I want to take listeners on a journey from drawing changes in the OpenStreetMap editor all the way until vectors are uploaded to from memory to GPUs.

Like outlined in the abstract, I want to cover multiple topics:

* Foundations of digital maps (How to determine which data should be loaded? What are vector and raster tiles?)
* Show the technology stack which allows us to design and develop a cross-platform map renderer (Web, Mobile, Desktop)

