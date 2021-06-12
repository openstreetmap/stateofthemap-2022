---
layout: session
title: "Collection and use of data about entrances of buildings"
code: "W7FP3J"
speaker_names_with_affiliations: ["Tuukka Hastrup"]
room: "Track 1 - Talks"
length: "20"
time: "Saturday, 11:30"
time_iso: "2021-07-10T11:30:00Z"
resources: []
recording: True
---
True door-to-door navigation requires us to accept that people don"t really visit housenumbers, they visit amenities and apartments via specific building entrances. The significance of this difference varies and is greatest in cities with unoptimal address schemes, for people with accessibility needs and for delivery drivers quickly visiting lots of unfamiliar recipients. 

City of Helsinki in Finland uses OLMap to take photos of each entrance to a building, to correct the GPS location of the entrance, to record the address and other properties of the entrance as well as to facilitate mapping this information and the access paths in OSM. Last year, the city employed some secondary school students as mappers. Over 6000 images including 5762 entrances, 1767 flights of steps, 645 barriers and 241 info boards were contributed to the 30000 entrances mapped in Helsinki. A new batch of students will be employed this summer.

Using Gatesolve, delivery drivers can take advantage of the address, entrance, and accessibility data collected and mapped in OSM. To limit visual clutter, the app includes zoom-dependent cartography of the entrances. The search finds entrance-level addresses and the routing function visualises any steps and barriers on the way to the entrances.

An entrance typically doesn"t have a unique housenumber, so it"s important to also map tags such as &#34;addr:unit&#34;, &#34;addr:flats&#34; or &#34;ref&#34; when appropriate. When these are not available, the different entrance types, access values etc. can help distinguish between entrances.

If a path without stairs has been mapped through to an entrance, we assume there are no stairs, but if there is any gap between the path and the entrance, we communicate uncertainty.

Entrances inside as opposed to along building outlines cause troubles for us. For example, there are entrances inside building passages and under hanging roofs. Mapping these entrances along &#34;building:parts&#34; can clarify this, but it"s disproportionately laborous as well as prone to topological mistakes which result in inaccurate cartography.

We continue to develop the apps. For instance, all the mapping this far has been done in the iD editor, but custom mapping functionality may be necessary to feasibly support explicitly linking amenities to corresponding entrances via the proposed &#34;associated_entrance&#34; relations.
