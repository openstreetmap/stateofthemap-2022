---
layout: qa
title: "Drones for Community Mapping"
code: "8JQ7PY"
---

1.  Are your drone images also being uploaded to Wikimedia Commons, for
    use on Wikipedia? - Andy Mabbett, @pigsonthewing
    1.  Not currently, but many are posted on OpenAerialMap under open
        licenses. -Eugene
    2.  this the imagery in the slide:
        <https://map.openaerialmap.org/#/121.13703299999999,16.93503259011358,17/square/13230132221/5d29ec177a18fd0005e2978e?resolution=high&_k=kgkfae>
    3.  Arenda imagery:
        <https://map.openaerialmap.org/#/121.11188650131226,14.537061956768639,15/square/13230312200133113/5dad0e1c16c43b00058d0262?resolution=high&_k=kizu9i>
        -maning
2.  How do you produce DTM, are you sing Pix4D and what are the quick
    procedure
    1.  Yep! I used Pix4D to generate DTM. You can check this diary
        entry I did for the Lupang Arenda example:
        <https://www.openstreetmap.org/user/geoleighyers/diary/391138>
3.  Is there open source software for processing drone images?  Pix4d is
    not open source.
    1.  Yes, you can OpenDroneMap which is opensource. -maning &lt;3
    2.  do you have any exeperionce
        1.  The OSM community in the Philippines have a bit of
            experience using OpenDroneMap and we are now experimenting
            with various settings to try and generate optimal orthophoto
            maps.
4.  Do you have the base map of Batad uploaded online somewhere?
    1.  Yep, you can check here:
        <https://map.openaerialmap.org/#/121.13703299999999,16.93503259011358,17/square/13230132221/5d29ec177a18fd0005e2978e?resolution=high&_k=kgkfae>
5.  This is awesome work! What were the reactions of the local
    communities that you worked with? Were they generally cooperative?
    Did they like the output when you shared it with them?
    1.  For Batad, they do not like drones in the area because it was
        noisy. But after the team explained it to the people, they were
        okay with it. We explained as much as we can why we need to get
        the data for research purposes and for their use as well.
    2.  For Lupang Arenda, the drone mapping was actually a request of
        the local government and they are now using the results of
        mapping in OSM as part of their rendering of public services.
        great to hear, thanks!
    3.  more info about this community collab:
        <https://github.com/OSMPH/papercut_fix/issues/54>
        1.  thanks! great to see that there's a lot of discussion about
            this!
6.  Are there privacy concerns (in case individual human beings are
    visible on the images) - do you blur these images, or ask people for
    their consent?
    1.  the 10cm resolution is not sharp enough to identify faces/people
        1.  Yep I agree.
7.  Is there any manual work for removing buildings for DTM, or
    everything done by software.
    1.  To enhance DTM data, WhiteBoxTools' RemoveOffTerrainObjects
        module was recommended by a colleague.
    2.  This is done automatically by software. Note that DTM is not
        super accurate because it requires the software recognizing
        trees and buildings and this is not very accurate. But the DSM
        is useful.
        1.  So the DTM is calculated from parallax between images?
            1.  Yes! Pix4D and OpenDroneMap uses computer vision
                techniques to determine the "3D" shapes of objects and
                uses that to calculate the DSM.
8.  Are there privacy concerns about objects visible on private ground
    (in backyards, e.g.) not visible from the street level?
    1.  In the works that I've done, we have proper coordination with
        the government officials down to the local community leaders to
        explain what we're collecting. As much as possible we
        communicate with the community what we're doing and collecting.
        So far, I haven't had this before. - Leigh
9.  Do you have any equipments to adjust positioning like RTK or
    something?
    1.  The drone itself has GPS capabilities to get the XYZ values. If
        the project / area requires higher accuracy in horizontal /
        vertical location, GPS Survey or adding GPS markers will help.
    2.  We only rely on the GPS/GNSS technology included inside the
        drones.
10. Great work! How do you choose locations/projects? What will be your
    next project?
    1.  Usually from friends from the geospatial community ask us to map
        out areas. I team up with other drone pilots, OpenStreetMap PH
        community or involve Philippines Flying Labs to do the mapping. 
        Currently, I don't have a next project due to the Corona Virus
        pandemic. Hopefully by next year, I can map again.
11. How much complex to geo-reference drones' shots?
    1.  All drone captured images have the location in its exif
        metadata.  All images can just be in a single directory and the
        software can take care of the stitching and georeferencing. 
        This is the same for proprietary and open source tools.
    2.  There are a few approaches to improve quality like taking
        nadir/perpendicular + oblique.  But in most cases, nadir images
        with 60-80% overlap will generate good results. -maning
        1.  Thanks for this sir!
12. What's the cost of such drones?
    1.  Oh it's such a huge range! It ranges from 1500 USD to 25,000
        USD. hehe. - Leigh
13. What is your message for girls all around the world who want to
    learn to fly a drone?
    1.  Go fly and enjoy it! Don't be afraid of the technicalities of
        it. :)
    2.  Go fly, and enjoy it (answer from Leigh) If people give you
        reasons not to, don't listen to them too hard (indiebio)
        1.  Why not "listen to them if they provide a reasonable
            explanation, and then make an informed decision taking into
            account this information" Would this require a different
            answer for women vs men?
            1.  (I'm a girl and I would think yes - indiebio)
            2.  There is good reason to encourage different groups of
                people, but that's a question for a diversity talk
                (Gregory).



-   You are an inspiration for women all over our communities and seeing
    you giving a talk about a highly technical topic gives us
    motivation.
-   Thank You for the talk, and your time working on this project -
    Natfoot
-   I need to do more of this. Done quite a bit of the photogrametery
    simalar to pix4D from the ground using a poleand a camera. GoPro
    cameras work well as they have a gps.  You can do it! happy to help
    you as well!
-   \[There's a problem with audio feedback - maybe encourage presenters
    to use earphones?\]
    -   yes, please

