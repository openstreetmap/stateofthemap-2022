---
voc: https://media.ccc.de/v/sotm2022-18479-evolving-the-osm-data-model
recordings: [{'size': 116, 'length': 1953, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2022-18479-eng-Evolving_the_OSM_Data_Model_webm-hd.webm', 'state': 'new', 'folder': 'webm-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2022-09-19T11:39:07.456+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/webm-hd/sotm2022-18479-eng-Evolving_the_OSM_Data_Model_webm-hd.webm', 'url': 'https://api.media.ccc.de/public/recordings/61813', 'event_url': 'https://api.media.ccc.de/public/events/22ea6b83-4305-5f06-9996-b2f0e4a5408e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 61, 'length': 1953, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2022-18479-eng-Evolving_the_OSM_Data_Model_webm-sd.webm', 'state': 'new', 'folder': 'webm-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2022-09-19T11:17:57.142+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/webm-sd/sotm2022-18479-eng-Evolving_the_OSM_Data_Model_webm-sd.webm', 'url': 'https://api.media.ccc.de/public/recordings/61807', 'event_url': 'https://api.media.ccc.de/public/events/22ea6b83-4305-5f06-9996-b2f0e4a5408e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 29, 'length': 1954, 'mime_type': 'audio/mpeg', 'language': 'eng', 'filename': 'sotm2022-18479-eng-Evolving_the_OSM_Data_Model_mp3.mp3', 'state': 'new', 'folder': 'mp3', 'high_quality': False, 'width': 0, 'height': 0, 'updated_at': '2022-09-19T10:59:03.907+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/mp3/sotm2022-18479-eng-Evolving_the_OSM_Data_Model_mp3.mp3', 'url': 'https://api.media.ccc.de/public/recordings/61797', 'event_url': 'https://api.media.ccc.de/public/events/22ea6b83-4305-5f06-9996-b2f0e4a5408e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 42, 'length': 1953, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2022-18479-eng-Evolving_the_OSM_Data_Model_sd.mp4', 'state': 'new', 'folder': 'h264-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2022-09-19T10:58:16.883+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/h264-sd/sotm2022-18479-eng-Evolving_the_OSM_Data_Model_sd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/61796', 'event_url': 'https://api.media.ccc.de/public/events/22ea6b83-4305-5f06-9996-b2f0e4a5408e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}, {'size': 72, 'length': 1953, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2022-18479-eng-Evolving_the_OSM_Data_Model_hd.mp4', 'state': 'new', 'folder': 'h264-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2022-09-19T10:54:14.213+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2022/h264-hd/sotm2022-18479-eng-Evolving_the_OSM_Data_Model_hd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/61793', 'event_url': 'https://api.media.ccc.de/public/events/22ea6b83-4305-5f06-9996-b2f0e4a5408e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2022'}]
layout: session
title: "Evolving the OSM Data Model"
code: "W3AGY8"
speaker_names: ['Jochen Topf']
affiliations: None
room: "Auditorium A"
length: "20"
time: "Friday, 15:30"
time_iso: "2022-08-19T13:30:00Z"
resources: [{ description: "Slides", url: "/attachments/W3AGY8_2022-sotm-jochen-topf-osm-data-model_BppirTK.pdf" }]
recording: True
---

The OSM data model with its nodes, ways, and relations has done an amazing job for us over the years. It has seen very little changes since relations were introduced 15 years ago. But there are some real problems with the data model. With the experience of those 15 years behind us, its time to tackle some improvements.

This talk will outline the problems with the data model, show ideas for improvements, and discuss possible ways that can move us forward step by step.

<hr>

The OSM data model is quite different from the &#34;Simple Feature&#34; data model used by most &#34;geo&#34; software. It has some great features, like the open tagging model, which has proven to be a great enabler for all sorts of innovations. But the data model also has its problems. Most often named are the missing area data type and the cumbersome geometry building needed for ways and relations based on their member nodes. This makes use of the OSM data more difficult, more expensive, and slower than it needs to be.

There has been some discussions on these topics over the years, mostly after my talk in 2018 at the SotM in Milano, but work on this has stalled. Recently the OSMF Engineering Working Group has taken up this topic and payed me to do a study on the problems with the data model and possible ways forward. This talk will present the findings and should jumpstart the discussions around this in the OSM community.

