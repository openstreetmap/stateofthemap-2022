---
layout: session
title: "Linting the map together: Collaborations of Mapbox Data RAVE and OpenStreetMap Communities"
code: "RSLM3H"
speaker_names_with_affiliations: ["Vlada Boitsik"]
room: "Track 1 - Talks"
length: "20"
time: "Friday, 20:45"
time_iso: "2021-07-09T20:45:00Z"
resources: []
recording: True
---
In October 2020, as part of on-going work to improve the quality of OpenStreetMap data, Mapbox Data RAVE employed osmlint-osmium and osmlint to detect road network data issues in Germany, France, Belgium, Netherlands, and the USA. We found significant issues that impact auto navigation, and variance depending on past editing activities of the community and corporate members in each country.

We began our work in each place in conversation. Sometimes we were met with friendliness, other times skepticism. We learned to respect local language conventions, which sometimes meant using machine translation, and this did help greatly. The preferred and active communication channels varied as well, from mailing lists, to forums, to IRC and Slack, to the Wiki and GitHub issues. For documentation, we took an “all of the above” approach, making sure to reflect adaptations in approach in all the spaces.

Technically we worked on 10 categories of mistakes: crossing highways, crossing highway bridges, impossible angle, island highways, impossible oneways, mixed layer and 4 categories connected with turn restrictions. We used all available ground truth sources to determine if an edit was needed, and tracked those edits with a changeset comments hashtags for our team and each country. 

So far we have reviewed more than 26,000 issues and fixed almost 55% of them. Hoping that this is just the beginning of coordination with communities and the Data RAVE team.
