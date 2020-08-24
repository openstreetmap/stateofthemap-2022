---
layout: qa
title: "Identify map problems in OSM by connectivity check"
code: "URVEBF"
---

Please feel free to start writing questions before the end of the talk
and remind to rename yourself :)

Speaker: Evan Hossain (
<https://www.linkedin.com/in/evan-hossain-ab6691a9> )
Chair: Lorenzo Stucchi (@LorenzoStucchi)

Questions:

1.  \[DONE\] Why do you need a check in \_directed\_ graph? in my
    validar I've implemented connectivity check using non-directed graph
    (just ignoring oneway tag), the algorithm to find islands(isolated
    sub-graphs) becomes much more simple, but results are practically
    the same  (Kirill aka Zkir)
    1.  You do not really need to analyze oriented graph. just analyze
        connectivity. :)
2.  \[DONE\] Could you explain wrong direction ? (both way seem
    connected by the same node)
3.  \[DONE\] Any opensource code repo?  And How We can adapt in other
    country?
4.  \[DONE\] User: Transport for Cairo.  Do wrong directions (opposing
    directions) cause disconnectivity, thus captured by the algorithm?
5.  \[DONE\] Are you concentrating solely on the car routing (profile)? 
    -- Stefan K.
6.  Profiles matter IMHO for pedestrian areas / plazas (with bicycle
    access, unidirectional) which are a special case for routing
7.  \[DONE\] How we can use his reversed algorith for COVID ?  make a
    more social distance ?


Comments:

1.   Yup, with all those trees and clouds, there are just a few shreds
    of roads I can map from imagery.
    1.  Use LIDAR!
2.  When you are finished with roads, get to work on house address
    number quality too...
3.  You can contruibue all this to iD editor's checker!

