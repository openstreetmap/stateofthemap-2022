---
layout: session
title: "Overpass API since 10 years"
code: "FV8QGF"
speaker_names_with_affiliations: ['Dr. Roland Olbricht']
room: "Track 1 - Talks"
length: "20"
time: "Sunday, 17:15"
time_iso: "2021-07-11T17:15:00Z"
resources: []
recording: True
---
Since now 10 years, the Overpass API allows to query the OpenStreetMap data.
This is reason enough to compare the OpenStreetMap of then to the OpenStreetMap of now
and to show how OpenStreetMap and the Overpass API have changed or not changed over that timespan.

For this purpose I will present an overview:

With which requests are the public instances of the Overpass API actually used?
The Overpass API has been intended for compound queries for the public transit data model of OpenStreetMap,
but actually got popular for the simpler tag queries on bounding boxes.
The provisions for an area data type have never materialized.

How has it protected itself and how does it now protect itself against excessive load?
I have always been proud that the service runs on ordinary server hardware and nothing huge,
but still can give every user a meaningful amount of computation time.
The necessary measures to curb the greedy and the stupid have evolved over time.

Which requests for features and questions have been addressed to me as the developer?
Basically everything we use now has been requested by users of the service.
Probably the best idea has been to change from the longish XML based query language to the now much shorter QL based language.
