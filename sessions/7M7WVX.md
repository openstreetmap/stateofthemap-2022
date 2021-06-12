---
layout: session
title: "How StreetComplete handles edits"
code: "7M7WVX"
speaker_names_with_affiliations: ["Tobias Zwick"]
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
