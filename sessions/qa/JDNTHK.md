---
layout: qa
title: "Minutely Extracts: Tools for nimble editing and downloading"
code: "JDNTHK"
---

Hello Mappers :) This is Brandon, the presenter. I'm looking forward to
your questions!
GitHub Repo: <http://github.com/protomaps/OSMExpress>
Documentation: <https://protomaps.com/docs/osmexpress>

**Questions:**

1.  Asking this in advance of the session, so apologies if you answer
    this: What communities, sectors, or use cases for Minutely Extracts
    and OSMX have been underutilized so far that you would encourage, in
    your view? (What are the new limits of ME vs. similar bounds queries
    in existing tools e.g. Overpass, OSM Extract?) -Thad
    1.   REPLY: use cases I have in mind are live-updated OSM statistics
        or vandalism detection; I don't work on these topics though, so
        hope that developers who do can use these tools. The limit of
        100m nodes on ME is arbitrary and based on a coarse estimate
        performed outside osmx; you can exceed this limit if you run the
        program yourself.
2.  \[DONE\] Would you be ok sharing the graph simplification tricks?
    (Already answered on Twitter)
3.  Do you have books to recommend to a developer with little experience
    in GIS (but with some general experience and an ok math background).
    I'd like to learn and be capable of doing the same kind of work as
    you but don't know where to start
    1.  REPLY: I have very little GIS background before starting to work
        with OpenStreetMap! I think there’s lots of opportunities for
        writing OSM tooling in efficient programming languages like C++,
        Go, Rust so I would recommend diving into one of those
4.  Would it be possible to support requesting minute extracts by
    geographic region, a bit like the geofabrik polygons? Or with an
    arbitrary Nominatim query? - Guillaume
    1.  REPLY: Yes, this is something i'm working on, but becomes
        challenging for relations with thousands of nodes and above
        1.  Cool, thanks :)
5.  What do you think are the advantages of Overpass over OSMExpress?
    1.  REPLY: Overpass has tons of features for interactive querying
        and also does deep "interpretation" of OSM objects into
        polygons, etc. osmx does none of that - it's just a file
6.  I had a break in the internet connection during the talk. Is there a
    difference compared to the download function of JOSM?
    1.  REPLY: yes, you can download up to 100 million nodes; however,
        untagged nodes don't have metadata beyond version number.
    2.  You can re-watch all the talks at
        <https://streaming.media.ccc.de/sotm2020/>


**Comments:**


1.  "MapCook-Bro". Nice.

