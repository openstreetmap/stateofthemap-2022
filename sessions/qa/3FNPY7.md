---
layout: qa
title: "Ranks for Rendering"
code: "3FNPY7"
---

Add questions here

1.  What are the rules for using third party data in OSM?
2.  If OSM features are tagged with their Wikidata items, can you use
    data stored in Wikidata to influence ranking? For example, number of
    passengers for airports. +1
3.  With increasing render options, do render managers share these
    learnings easily?
4.  Do you think that using vector tiles would help improve the
    cartography? Or is the solution to add better ranks and to just keep
    working on it?
    1.  thanks for the answer! just putting it here for anyone's benefit
        1.  ANSWER: the cartography problems still exist whether you use
            raster tiles or vector tiles
5.  There are railway stations with airport IATA codes (e.g. New York
    stations). The use of IATA code to enhance rendering becomes hard to
    apply in some cases.
6.  Could you use the number of terminals to classify airport
    importance?
7.  Rendering of waterways labels is very hard to achieve because of the
    already explained reasons. Since centuries, the labeling of
    waterways based on lenght/size/flow is a basic part of a map. How to
    solve this using OSM data?
8.  Would it be so bad to have mappers record a relative importance,
    something like a "scale\_rank" or so?
    1.  Isn't this going back to the old debate about adding subjective
        data into OSM? Mappers are still complaining about the
        smoothness=\* tag.
9.  Have you considered the number of gates within an airport area for
    estimate its importance?
10. Could you make the ranking relative to the highest visible rank in
    the area rendered?



-   Feedback (not a question) - Thank you for the interesting talk.
    <https://github.com/Wikidata/Wikidata-Toolkit> may be interesting
    for importing wikidata into PostgreSQL (unsure about the performance
    of this tool). <https://wiki.openstreetmap.org/wiki/Wikidata> lists
    tools and there was a talk last year:
    <https://2019.stateofthemap.org/attachments/GUUUYW_OpenStreetMap_and_Wikidata_-_Awesome_Together.pdf>
    +1, thanks! (it also mentions some concerns around data licensing,
    which could be important) (which in my regard should be addressed
    ASAP ;-\] it'd be so nice to have WIkidata and OSM in-sync)
    -   The 2 licenses are so far away from each other. I don't see this
        happening. Yeah :-(
        -   But it's mostly an issue if you want to move data from one
            to the other. If you want to use a Wikidata property to
            guide your rendering, I don't think it's a stumbling block.
            -   My perspective is mostly from the WIkidata Query Service
                (WDQS), in which it would be nice to have OSM data over
                there.
                -   You can, as long as you give credit, can't you?
                    -   From how I understand the discussion (see Wiki
                        link above), import is disallowed. Linkage OK.
                        (Before I lose you, do you have other info, or
                        another understanding?)
-   Congrats Michael, well done!!+5

