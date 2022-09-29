---
voc: https://media.ccc.de/v/sotm2022-18516-the-maposmatic-apis-generate-printable-maps-from-your-own-application
recordings: [{'size': 79, 'length': 1357, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_webm-hd.webm', 'state': 'new', 'folder': 'webm-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2022-09-25T16:32:05.591+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/webm-hd/sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_webm-hd.webm', 'url': 'https://api.media.ccc.de/public/recordings/62007', 'event_url': 'https://api.media.ccc.de/public/events/24370f9a-2ac4-5467-8fa9-dfe56e7af049', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 39, 'length': 1357, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_webm-sd.webm', 'state': 'new', 'folder': 'webm-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2022-09-25T16:16:04.850+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/webm-sd/sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_webm-sd.webm', 'url': 'https://api.media.ccc.de/public/recordings/62003', 'event_url': 'https://api.media.ccc.de/public/events/24370f9a-2ac4-5467-8fa9-dfe56e7af049', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 27, 'length': 1357, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_sd.mp4', 'state': 'new', 'folder': 'h264-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2022-09-25T16:03:03.513+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/h264-sd/sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_sd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/61998', 'event_url': 'https://api.media.ccc.de/public/events/24370f9a-2ac4-5467-8fa9-dfe56e7af049', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 20, 'length': 1357, 'mime_type': 'audio/mpeg', 'language': 'eng', 'filename': 'sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_mp3.mp3', 'state': 'new', 'folder': 'mp3', 'high_quality': False, 'width': 0, 'height': 0, 'updated_at': '2022-09-25T16:02:03.060+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/mp3/sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_mp3.mp3', 'url': 'https://api.media.ccc.de/public/recordings/61997', 'event_url': 'https://api.media.ccc.de/public/events/24370f9a-2ac4-5467-8fa9-dfe56e7af049', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 47, 'length': 1357, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_hd.mp4', 'state': 'new', 'folder': 'h264-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2022-09-25T15:58:16.380+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/h264-hd/sotm2022-18516-eng-The_MapOSMatic_APIs_-_generate_printable_maps_from_your_own_application_hd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/61993', 'event_url': 'https://api.media.ccc.de/public/events/24370f9a-2ac4-5467-8fa9-dfe56e7af049', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}]
layout: session
title: "The MapOSMatic APIs - generate printable maps from your own application"
code: "HBBZKV"
speaker_names: ['Hartmut Holzgraefe']
affiliations: None
room: "Auditorium A"
length: "20"
time: "Saturday, 10:00"
time_iso: "2022-08-20T08:00:00Z"
resources: [{ description: "Presentation Slides", url: "/attachments/HBBZKV_2022-SOTM-Print-Maps-API.plain_Uya0cD4.pdf" },{ description: "Presentation Handout", url: "/attachments/HBBZKV_2022-SOTM-Print-Maps-API.handout_Lqn71dq.pdf" }]
recording: True
---

The MapOSMatic web frontend allows to create printable maps from OSM
data interactively. This is not the only way to use its rendering
backend, it is also possible to directly use its ocitysmap Python
library to render maps from your own Python code and a local
stylesheet and database setup, or to use the REST-like API of the web
frontend to send automated render requests to a MapOSMatic web
instance from almost any programming language without any local setup
effort.

The presentation will give a short overview of both API variants,
showing the different options to interact with the MapOSMatic render
infrastructure programmatically.

As example applications an alternative neighbourhood

