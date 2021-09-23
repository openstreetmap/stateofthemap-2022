---
voc: https://media.ccc.de/v/sotm2021-10044-how-streetcomplete-handles-edits
recordings: [{'size': 125, 'length': 1602, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2021-10044-eng-How_StreetComplete_handles_edits_webm-hd.webm', 'state': 'new', 'folder': 'webm-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2021-09-21T20:52:38.472+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2021/webm-hd/sotm2021-10044-eng-How_StreetComplete_handles_edits_webm-hd.webm', 'url': 'https://media.ccc.de/public/recordings/55016', 'event_url': 'https://media.ccc.de/public/events/bedab0b4-e8be-59aa-afe4-8abf26b8675c', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2021'}, {'size': 60, 'length': 1602, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2021-10044-eng-How_StreetComplete_handles_edits_webm-sd.webm', 'state': 'new', 'folder': 'webm-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2021-09-21T20:28:34.515+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2021/webm-sd/sotm2021-10044-eng-How_StreetComplete_handles_edits_webm-sd.webm', 'url': 'https://media.ccc.de/public/recordings/55014', 'event_url': 'https://media.ccc.de/public/events/bedab0b4-e8be-59aa-afe4-8abf26b8675c', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2021'}, {'size': 44, 'length': 1602, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2021-10044-eng-How_StreetComplete_handles_edits_sd.mp4', 'state': 'new', 'folder': 'h264-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2021-09-21T20:13:33.264+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2021/h264-sd/sotm2021-10044-eng-How_StreetComplete_handles_edits_sd.mp4', 'url': 'https://media.ccc.de/public/recordings/55013', 'event_url': 'https://media.ccc.de/public/events/bedab0b4-e8be-59aa-afe4-8abf26b8675c', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2021'}, {'size': 24, 'length': 1602, 'mime_type': 'audio/mpeg', 'language': 'eng', 'filename': 'sotm2021-10044-eng-How_StreetComplete_handles_edits_mp3.mp3', 'state': 'new', 'folder': 'mp3', 'high_quality': False, 'width': 0, 'height': 0, 'updated_at': '2021-09-21T20:10:32.993+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2021/mp3/sotm2021-10044-eng-How_StreetComplete_handles_edits_mp3.mp3', 'url': 'https://media.ccc.de/public/recordings/55011', 'event_url': 'https://media.ccc.de/public/events/bedab0b4-e8be-59aa-afe4-8abf26b8675c', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2021'}, {'size': 107, 'length': 1602, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2021-10044-eng-How_StreetComplete_handles_edits_hd.mp4', 'state': 'new', 'folder': 'h264-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2021-09-21T20:08:35.499+02:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2021/h264-hd/sotm2021-10044-eng-How_StreetComplete_handles_edits_hd.mp4', 'url': 'https://media.ccc.de/public/recordings/55009', 'event_url': 'https://media.ccc.de/public/events/bedab0b4-e8be-59aa-afe4-8abf26b8675c', 'conference_url': 'https://media.ccc.de/public/conferences/sotm2021'}]
layout: session
title: "How StreetComplete handles edits"
code: "7M7WVX"
speaker_names_with_affiliations: ['Tobias Zwick']
room: "Track 1 - Talks"
length: "20"
time: "Saturday, 15:00"
time_iso: "2021-07-10T15:00:00Z"
resources: []
recording: True
---
StreetComplete is known as an app to easily contribute selected data to OSM on the go. 

The simple interface could make it appear that the technical implementation is equally simple. It is maybe a common misconception that things that look easy to the user are also lighter in terms of code complexity. But under the hood, it is anything but.

For example, amongst other things, the app has a unique way to avoid and to automatically resolve conflicts when uploading data to OSM. For an app that promises its users to work completely offline and thus automatically stores unsynced edits for any duration before upload, this is very useful to have.

Furthermore, it comes with the ability to undo edits in any order (not just the last) and even undo most edits after they have been synced with OSM already.

This talk shall give you an architectural overview over how StreetComplete enables its users to do these things.
It could serve other editor developers as inspiration, however, most technical concepts in this app are probably not well applicable to be used in a general OSM editor, as StreetComplete vastly limits its users what they can do and therefor we can make certain assumptions about how the app is used.
