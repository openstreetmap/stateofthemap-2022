---
youtube: RxmkNAHPrPk
voc: https://media.ccc.de/v/sotm2020-4339-mapcampaigner-redesign-the-data-quality-monitor-for-osm
recordings: [{'size': 51, 'length': 1516, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_sd.mp4', 'state': 'new', 'folder': 'h264-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2020-07-15T01:13:44.438+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2020/h264-sd/sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_sd.mp4', 'url': 'https://media.ccc.de/public/recordings/47472', 'event_url': 'https://media.ccc.de/public/events/19380c6e-1f22-5bb5-991b-718ba7adc6da', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2020'}, {'size': 176, 'length': 1516, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_webm-hd.webm', 'state': 'new', 'folder': 'webm-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2020-07-15T01:13:18.440+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2020/webm-hd/sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_webm-hd.webm', 'url': 'https://media.ccc.de/public/recordings/47471', 'event_url': 'https://media.ccc.de/public/events/19380c6e-1f22-5bb5-991b-718ba7adc6da', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2020'}, {'size': 66, 'length': 1516, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_webm-sd.webm', 'state': 'new', 'folder': 'webm-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2020-07-15T01:11:08.550+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2020/webm-sd/sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_webm-sd.webm', 'url': 'https://media.ccc.de/public/recordings/47470', 'event_url': 'https://media.ccc.de/public/events/19380c6e-1f22-5bb5-991b-718ba7adc6da', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2020'}, {'size': 23, 'length': 1516, 'mime_type': 'audio/mpeg', 'language': 'eng', 'filename': 'sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_mp3.mp3', 'state': 'new', 'folder': 'mp3', 'high_quality': False, 'width': 0, 'height': 0, 'updated_at': '2020-07-15T00:56:47.526+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2020/mp3/sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_mp3.mp3', 'url': 'https://media.ccc.de/public/recordings/47467', 'event_url': 'https://media.ccc.de/public/events/19380c6e-1f22-5bb5-991b-718ba7adc6da', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2020'}, {'size': 145, 'length': 1516, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_hd.mp4', 'state': 'new', 'folder': 'h264-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2020-07-15T00:50:51.160+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2020/h264-hd/sotm2020-4339-eng-Mapcampaigner_Redesign_The_Data_Quality_Monitor_For_OSM_hd.mp4', 'url': 'https://media.ccc.de/public/recordings/47464', 'event_url': 'https://media.ccc.de/public/events/19380c6e-1f22-5bb5-991b-718ba7adc6da', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2020'}]
layout: session
title: "Mapcampaigner Redesign: The Data Quality Monitor For OSM"
code: "VJS3LC"
speaker_names_with_affiliations: ["Jorge Martinez"]
room: "Track 1"
length: "20"
time: "Saturday, 16:30"
time_iso: "2020-07-04T16:30:00Z"
resources: []
recording: True
pad: https://pad.sotm.bitcast.co.za/p/mapcampaigner-redesign-the-data-quality-monitor-fo
---
When we talk about a mapping campaign, it generally has specific characteristics:
Desire to collect geospatial data for a purpose.
Define an area of interest.
Define a set of features and attributes to collect.
The period of time of the campaign
Group of people to collect the data. Could be highly trained staff members or volunteers.

It would sound simple. However, it is possible to find challenges in difficult places. For instance, how to crowdsource precise locations and specific attributes of every school in Barranquilla, Colombia? Because some locations are inaccessible, it becomes difficult and costly to deploy people to the area to collect and validate the data. Many tools have been developed to address these challenges remotely, like OpenMapKit and Maps.me to collect data and do some quality assurance with JOSM, for instance. Despite this, these tools do not have the property to monitor specific features/attributes, define current status of the mapping campaign, or validate people contributing in an area.

Putting these challenges in mind, HOT designed the MapCampaigner tool. Users can track and measure the quality of many features such as schools, buildings and cafes at the same time. This mapping campaign will report users involved, missing tags, and percentage of completeness in an area for each attribute collected. Also, MapCampaigner has integrations with apps such as Maps.me and OpenMapKit

In this talk, I will walk through the tool, how it is used, and seek input for enhancements. Will show new features included in the latest user-centered redesign using  live demo. The schedule of this talk is the following:
Introduction and problem statement (5 minutes).
MapCampaigner features (5 minutes)
Examples and demo (5 minutes)
Conclusions and future work (5 minutes)
