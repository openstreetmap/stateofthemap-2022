---
layout: session
title: "News from osm2pgsql"
code: "7RWSWA"
speaker_names_with_affiliations: ["Jochen Topf"]
room: "Track 1 - Talks"
length: "20"
time: "Saturday, 16:30"
time_iso: "2021-07-10T16:30:00Z"
resources: []
recording: True
---
The osm2pgsql has been around for a long time. Since 2006 it is used to import OSM data into PostgreSQL/PostGIS databases for rendering and other uses. In the last years there have been a lot of improvements to osm2pgsql. With the new &#34;Flex&#34; output, osm2pgsql is now much more versatile which allows new applications.

The talk will be about the new developments in osm2pgsql und show how to use the new features. Osm2pgsql is used for rendering bitmap tiles for many maps, including the main OSM map and many others. But it can also be used to import OSM data for generating vector tiles and for many other use cases. It is now possible to tell osm2pgsql exactly what output tables with what fields to create in the database. Transformations from the OSM tags to more or less any format you need in your database can be defined in Lua code. Together with the powerful SQL query language in PostgreSQL and the geometric algorithms in the PostGIS plugin, this makes all sorts of analytical processing possible. Osm2pgsql can be used to import small OSM extracts quickly for one-off processing or run a minutely updated planet-wide database on a reasonably-sized machine making OSM data processing accessible for everybody.
