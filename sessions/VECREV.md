---
voc: https://media.ccc.de/v/sotm2022-18246-0-maplibre-rs-cross-platform-map-rendering-using-rust
recordings: [{'size': 84, 'length': 988, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_webm-hd.webm', 'state': 'new', 'folder': 'webm-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2022-09-19T14:00:05.675+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/webm-hd/sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_webm-hd.webm', 'url': 'https://api.media.ccc.de/public/recordings/61840', 'event_url': 'https://api.media.ccc.de/public/events/1d67a8c1-17e6-5e30-965e-5d72311cd6b7', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 38, 'length': 988, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_webm-sd.webm', 'state': 'new', 'folder': 'webm-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2022-09-19T13:48:04.244+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/webm-sd/sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_webm-sd.webm', 'url': 'https://api.media.ccc.de/public/recordings/61838', 'event_url': 'https://api.media.ccc.de/public/events/1d67a8c1-17e6-5e30-965e-5d72311cd6b7', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 27, 'length': 987, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_sd.mp4', 'state': 'new', 'folder': 'h264-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2022-09-19T13:35:04.123+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/h264-sd/sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_sd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/61835', 'event_url': 'https://api.media.ccc.de/public/events/1d67a8c1-17e6-5e30-965e-5d72311cd6b7', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 15, 'length': 988, 'mime_type': 'audio/mpeg', 'language': 'eng', 'filename': 'sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_mp3.mp3', 'state': 'new', 'folder': 'mp3', 'high_quality': False, 'width': 0, 'height': 0, 'updated_at': '2022-09-19T13:34:03.348+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/mp3/sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_mp3.mp3', 'url': 'https://api.media.ccc.de/public/recordings/61834', 'event_url': 'https://api.media.ccc.de/public/events/1d67a8c1-17e6-5e30-965e-5d72311cd6b7', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 67, 'length': 987, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_hd.mp4', 'state': 'new', 'folder': 'h264-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2022-09-19T13:31:44.745+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/h264-hd/sotm2022-18246-eng-maplibre-rs_Cross-platform_Map_Rendering_using_Rust_hd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/61833', 'event_url': 'https://api.media.ccc.de/public/events/1d67a8c1-17e6-5e30-965e-5d72311cd6b7', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}]
layout: session
title: "maplibre-rs: Cross-platform Map Rendering using Rust"
code: "VECREV"
speaker_names: ['Max Ammann']
affiliations: MapLibre
room: "Workshops and Loop-Cinema - Room 103"
length: "20"
time: "Friday, 17:30"
time_iso: "2022-08-19T15:30:00Z"
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

