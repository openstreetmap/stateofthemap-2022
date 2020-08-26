---
layout: qa
title: "OSM Routing Evaluation"
code: "MJ8ZY8"
---

**Add questions here**


-   Ah, (my thought's from Mustard's introduction:) so by putting
    routing on OSM.org, OSM has made a conscious decision to go beyond
    just being a data creator. (Good.).
    -   Yantisa: Indeed, and I would love to see OSM communities use and
        develop routing (engine&data) that is best suited for their
        area.
-   Funny route choice: avoid all police stations.
    -   Yantisa: yes, true that! It is possible to make a route that
        avoid all police stations, especially all police station already
        well mapped ;)
-   Are the pedestrian ways and sidewalks well mapped on the area you
    evaluated? It's good to consider the connectivity of pedestrian ways
    to streets on this study.
    -   Yantisa: It depends, in Jakarta metro areas, the pedestrian is
        currently being well developed and tactile paving is starting to
        get common. In terms of mapping, these sidewalks is far from
        complete. In my scenario 2 talk, some of the sidewalk have been
        mapped (<https://overpass-turbo.eu/s/VMN)>. Unfortunately as you
        move outwards, pedestrian and sidewalks are not that well
        developed and not yet mapped.
-   How does OSRM prioritize in terms of road class? One wouldn't want
    to find themselves in dust tracks because it is a shorter distance.
    -   Yantisa: Just a disclaimer that I am not really familiar with
        OSRM, I do quite familiar with Graphhopper (GH). In GH, the
        higher a road classification it gets more priority. So motorway
        get the highest down to tracks as the lowest. More about road
        classification in OSM:
        <https://wiki.openstreetmap.org/wiki/Key:highway>
-   Are crime areas a concern?
    -   Yantisa: As far as I know, in default, the routing engine did
        not put it into consideration. Yet, it is fully possible for
        routing engine to avoid certain areas in their routing
        calculations.
-   Any specific attributes that we need to put into, to improve route
    for all of three route provider?+2
    -   Yantisa: Yes, road classification is the first one because it
        gives information to routing engine on which road to prioritize.
        Other tags will be quite useful, such as maxspeed, oneway or
        access restriction. Here is a good page that give more
        information:
        <https://wiki.openstreetmap.org/wiki/OSM_tags_for_routing>
-   Does Gojek (your company) use OSM for routing?+1
    -   Yantisa: we are currently still evaluating to adopt OSM and
        several other data sources as well as routing engine, stay tuned
        for any updates ;)
-   How does OSRM collect route data? is it done in participatory?
    -   Here are the tags that OSRM uses:
        <https://taginfo.openstreetmap.org/projects/osrm#tags> -maning
    -   Take note, \`highway=track\` is not used by OSRM. -maning
        -   Yantisa: thanks a lot, Maning! Ah interesting, since
            Graphhopper is still using track in its routing
            calculations.
-   Any opinions on Valhalla?
    -   Yantisa: Initially I want to include Valhalla in my comparison
        but because they did not have easily accessible web demo for
        routing thus I did not continue. Mapzen does have several
        interesting technology, Valhalla is one of them. Since Valhalla
        acquisition by Mapbox, I did not hear any more updates about it
        in OSM-talk or OSM forum.


Yantisa: Thanks everyone for your questions!

