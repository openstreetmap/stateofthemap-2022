---
layout: qa
title: "Measuring OpenStreetMap building footprint completeness using human settlement layers"
code: "YUM9PY"
---

[<span
class="underline">https://gisco-services.ec.europa.eu/distribution/v2/countries/distribution/TZ-region-01m-4326-2020.geojson</span>](https://gisco-services.ec.europa.eu/distribution/v2/countries/distribution/TZ-region-01m-4326-2020.geojson)

DOI: <https://doi.org/10.5281/zenodo.3923033>
Slides: <https://bit.ly/sotm2020-osm-completeness>
Code: <https://github.com/thinkingmachines/osm-completeness>

Science Mailing List:
<https://lists.openstreetmap.org/listinfo/science>

(It is considered polite to sign your name to questions.)

**Questions**

1.  \[DONE\] How long were you able to process the whole data in the
    Philippines? -Feye
2.  \[DONE\] You assume that the Facebook settlement layer is accurately
    depicting where built-up areas are. Did you verify that assumption
    against some known data in the Philippines? -- Frederik (this seems
    to somewhat conflict with question 4 - i was assuming that Facebook
    was AI'ing aerial imagery?)
3.  \[DONE\] You said that building data are required to "know where
    people live". But if you were e.g. an aid organisation wanting to
    find out where people live, could you not also look at
    landuse=residential or highway=residential objects in OSM - since
    these are easier to add for mappers than tracing buildings? --
    Frederik +1
4.  \[DONE\] The settlement layer focuses on mapping population, i.e.
    populated areas. Some areas have buildings but only non-residential
    ones, with zero population. Is that an issue for your method? +1
5.  \[DONE\] Does your method consider the different population density?
    Some buildings may have 1 storey, some may be skyscrapers, so a
    pixel in the settlement layer with a certain value for the
    population may mean different things - the same population can fit
    in one building or lots of them, depending on the number of floors.
6.  How difficult is to run your method for all countries?
7.  \[DONE\] (if time allows) Are you interpolating over the settlement
    data or assigning pixel-to-area? have you tried interpolation?
8.  \[DONE\] How do you evaluate Frederik Ramm's statement on volunteer
    vs. paid mapping, giving you've seen the talk yesterday. With
    sponsoring stopping, consequently the mapping stopping. -
    YaguraStation
9.  \[DONE\] Amazing work! Is it also possible to download the
    completeness datasets you generated for Phillipines and Madagascar?
    Would like to see it without going to run your wonderful code.
    Felix D. And me too please Janet
10. WorldPop takes into consideration the real population data based on
    the census (+ projections) and then assigns the 100m pixel value
    across those admin polygons. Did you consider the same?
11. \[DONE\] With the results for the Philippines, what are your
    recommendations for the local OSM community in terms of focus in
    mapping areas?


**Comments**

-   Things on Facebook are never free! They are only useable for those
    who are its customers and are tracked by it. Since OSM is a free
    project, Facebook is not a suitable tool for organizing things.
    Moreover, Facebook breaks the OSM rule and does not mention that its
    maps are from OSM.
    -   It is released under cc by 4.0
-   This is absolutely amazing! This can help our communities identify
    priority areas as well! **No building left behind!**
-   Thanks for the talk. There's **Audio-Feedback** during the Q&A from
    somewhere.
-   For those who are still interested in an intro to OSM and QGIS (like
    my lightning talk showed), see this free self-learning material:
    OpenSchoolMaps - www.openschoolmaps.org - Download PDFs 
    <https://tinyurl.com/openschoolmaps-zip-download> . -- Stefan Keller
    -   thank you! - indiebio
-   Authors are already aware of this, but for the benefit of the
    audience - another great dataset that can help in such analysis is
    the Global Human Settlement Layer (GHSL), produced by the European
    Commission - JRC: <https://ghsl.jrc.ec.europa.eu> -- Marco Minghini

