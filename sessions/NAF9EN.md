---
voc: https://media.ccc.de/v/sotm2022-18510-what-you-map-is-not-always-what-you-get
recordings: [{'size': 227, 'length': 3426, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_webm-hd.webm', 'state': 'new', 'folder': 'webm-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2022-09-19T12:48:11.109+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/webm-hd/sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_webm-hd.webm', 'url': 'https://api.media.ccc.de/public/recordings/61831', 'event_url': 'https://api.media.ccc.de/public/events/9e30959e-20c2-573d-b2a2-0ad93b513154', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 112, 'length': 3426, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_webm-sd.webm', 'state': 'new', 'folder': 'webm-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2022-09-19T12:01:06.669+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/webm-sd/sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_webm-sd.webm', 'url': 'https://api.media.ccc.de/public/recordings/61820', 'event_url': 'https://api.media.ccc.de/public/events/9e30959e-20c2-573d-b2a2-0ad93b513154', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 75, 'length': 3426, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_sd.mp4', 'state': 'new', 'folder': 'h264-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2022-09-19T11:26:05.332+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/h264-sd/sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_sd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/61811', 'event_url': 'https://api.media.ccc.de/public/events/9e30959e-20c2-573d-b2a2-0ad93b513154', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 52, 'length': 3426, 'mime_type': 'audio/mpeg', 'language': 'eng', 'filename': 'sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_mp3.mp3', 'state': 'new', 'folder': 'mp3', 'high_quality': False, 'width': 0, 'height': 0, 'updated_at': '2022-09-19T11:23:04.300+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/mp3/sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_mp3.mp3', 'url': 'https://api.media.ccc.de/public/recordings/61810', 'event_url': 'https://api.media.ccc.de/public/events/9e30959e-20c2-573d-b2a2-0ad93b513154', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 147, 'length': 3426, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_hd.mp4', 'state': 'new', 'folder': 'h264-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2022-09-19T11:03:50.736+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/h264-hd/sotm2022-18510-eng-What_you_map_is_not_always_what_you_get_hd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/61798', 'event_url': 'https://api.media.ccc.de/public/events/9e30959e-20c2-573d-b2a2-0ad93b513154', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}]
layout: session
title: "What you map is not always what you get"
code: "NAF9EN"
speaker_names: ['Sarah Hoffmann', 'Richard Fairhurst']
affiliations: None
room: "Auditorium A"
length: "40"
time: "Friday, 16:30"
time_iso: "2022-08-19T14:30:00Z"
resources: [{ description: "Slides", url: "/attachments/NAF9EN_sotm2022-tagging_5BVFgMo.pdf" }]
recording: True
---

OSM has an unrestricted tagging model. Mappers can invent and use any tags.
While this is part of OSM's success story, it has lead to a database where
the globe is described in ever greater detail. In this talk we want to
explore how users of OSM data handle a tagging model with so few constraints.
Richard, the owner of cycle.travel, and Sarah, maintainer of Nominatim, team
up to share their experiences of a decade of working with, and occasionally
fighting against, OSM's ever evolving tagging schema.

<hr>

The OSM tagging model has significantly evolved since the first streets of
London were put into the database. Not only are more and more different
objects in the database, we also capture more of their properties and want
to model ever finer nuances. This clashes with our goal to have one
database for the entire planet. The closer we look the more differences
between different regions there are. And to capture those the tagging has to
become even more complex.

Using the examples of the cycle tour planning site cycle.travel and the
search engine Nominatim, we explore the evolution of OSM tagging from
a data user's point of view. Looking at questions like

* where do data users get their information about tagging
* what kind of tagging can be practically used in software
* how to handle local defaults and assumptions
* how should OSM ideally document its tagging

