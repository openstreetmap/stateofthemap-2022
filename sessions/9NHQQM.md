---
layout: session
title: "osm2streets: Street networks with detailed geometry"
code: "9NHQQM"
speaker_names: ['Dustin Carlino']
affiliations: the Alan Turing Institute
room: "Auditorium A"
length: "20"
time: "Sunday, 10:00"
time_iso: "2022-08-21T08:00:00Z"
resources: []
recording: True
---

OpenStreetMap has many details about streets, but applications rendering or simulating lane-level detail face many challenges: determining lane properties along one street, calculating geometry of streets and junctions, handling motorway entrances, dual carriageways, dog-leg intersections, placement tags, and parallel sidewalks and cycleways. osm2streets is a new effort to produce a cleaned-up street network graph with geometry. It's a Rust library, designed to be integrated with browser apps like iD or native/Java apps like JOSM. The goal is to consolidate community efforts to solve these data transformation problems, and to produce high-detail vector maps and apps for improving lane tagging with immediate visual feedback.

