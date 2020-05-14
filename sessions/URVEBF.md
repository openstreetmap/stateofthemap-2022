---
layout: session
title: "Identify map problems in OSM by connectivity check"
code: "URVEBF"
speaker_names_with_affiliations: ["Evan Hossain"]
room: "Track 1"
length: "00:20"
time: "Sunday, 12:15"
time_iso: "2020-07-05T12:15:00Z"
resources: []
recording: True
---
In an ideal map, every point is reachable to another. Like any crowd-sourced product, it is a challenging goal for OSM to be ideal because the edits are from contributors with various backgrounds. For instance, only 98.59% of Singapore’s nodes are reachable to each other. This could cause significant problems when routing from one point to another for any business use case. In June 2019, some contributor mistakenly tagged one of the five major expressways  in Singapore with Access=No, which subsequently caused all the routing through the expressway to fail. 

In this talk, we address the issue  by using strongly connected component algorithms to identify such map problems and building a creative visualisation to help map analysts pinpoint the fix effortlessly. Using this technique, we identify map errors such as two one-way roads meeting each other with opposite directions;  duplicate nodes causing roads disconnected; parking lots not connected to main road network and more. The detected map errors spread everywhere on the map that motivates us to build a creative visualisation to help map analysts pinpoint the erroneous nodes/ways. Using this approach, we have fixed thousands of map problems in SEA.
