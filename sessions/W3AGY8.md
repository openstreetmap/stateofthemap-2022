---
layout: session
title: "Evolving the OSM Data Model"
code: "W3AGY8"
speaker_names_with_affiliations: ['Jochen Topf']
room: "Auditorium A - A001"
length: "20"
time: "Friday, 15:30"
time_iso: "2022-08-19T15:30:00Z"
resources: []
recording: True
---

The OSM data model with its nodes, ways, and relations has done an amazing job for us over the years. It has seen very little changes since relations were introduced 15 years ago. But there are some real problems with the data model. With the experience of those 15 years behind us, its time to tackle some improvements.

This talk will outline the problems with the data model, show ideas for improvements, and discuss possible ways that can move us forward step by step.

<hr>

The OSM data model is quite different from the &#34;Simple Feature&#34; data model used by most &#34;geo&#34; software. It has some great features, like the open tagging model, which has proven to be a great enabler for all sorts of innovations. But the data model also has its problems. Most often named are the missing area data type and the cumbersome geometry building needed for ways and relations based on their member nodes. This makes use of the OSM data more difficult, more expensive, and slower than it needs to be.

There has been some discussions on these topics over the years, mostly after my talk in 2018 at the SotM in Milano, but work on this has stalled. Recently the OSMF Engineering Working Group has taken up this topic and payed me to do a study on the problems with the data model and possible ways forward. This talk will present the findings and should jumpstart the discussions around this in the OSM community.

