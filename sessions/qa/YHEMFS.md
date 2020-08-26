---
layout: qa
title: "Assessing Global OpenStreetMap building completeness to generate large-scale 3D city models"
code: "YHEMFS"
---

**DOI:**
[**https://doi.org/10.5281/zenodo.3922285**](https://doi.org/10.5281/zenodo.3922285)

**Questions**

1.  <s>Wow! Further reading on tools?</s> found
    <https://github.com/osmbuildings/>  - YaguraStation
    1.  (I can't believe how much awesome stuff is going on, so happy
        :) - indiebio)
2.  How can we easily estimate building height while mapping? -
    Anonymous +2
3.  Can you discuss more about the feature importance for your random
    forest model in your study in the Netherlands? - ardieorden
    1.  ANS: number of stories
    2.  ANS: floor area
    3.  ANS: complexity of footprint
    4.  ANS: there's lots of other predictors, but the concern is how
        available those are globally
4.  Are cities in the Netherlands very similar for this to work? I could
    imagine it could be more complicated in countries with old and new
    cities?
5.  The examples shown all seem to assume a flat ground level.  Have you
    also tested estimation for cities on hills? +2
    1.  Answ: Flat terrain was assumed, as slope is not important in the
        netherlands. But to transfer, they will look into it. :)
6.  Can you use building shadows from satellite imagery to predict
    heights as you will have some buildings as control? +2
7.  Thanks very much for this very interesting talk! Have you also
    thought about elevation estimation from earth observation data, such
    as: SAR data from Sentinel 1 ? Since Radar data might also provide
    informaitons about building heights, while might be less accureate
    than 3D point cloud .
8.  Hello! Thanks and congratulations. Have you tried to apply
    image-recognition ML models on orthophotos to refine your
    predictions? I'm specifically thinking of CNN, but any other method
    also (also see question \#6 and \#9).
9.  what about estimating building hight with terrain photographs such
    as Mapillary repository? has it been done? +1
10. Exeter in the UK has around 35% 3D building coverage of the majority
    of buildings - it would be a good training set. Combined with other
    data we could see what works best. See this area for the Met Office
    as an example:
    <https://demo.f4map.com/#lat=50.7271961&lon=-3.4753034&zoom=19>
11. I  believe most of Netherlands have buildings between 1 and 3
    floors. Isn't the absolute error of 1 floor a bit big for that? --
    Ilya +2
12. Did you consider including national regulations on mandated distance
    spaces into the prediction model?
13. Isn't the geometry a bit "fuzzy"? some people map very thoroughly,
    others map basic footprints.+1 nice clarification :)
14. Can you explain once again how Landsat Raster is being used to
    predict completeness? ANS: He said they are not using raster data
    except for monitoring completeness of data  Yes, 2D footprint
    completeness. He definitely mentioned that!



**Comments**

-   Looking forward to see if this project will lead to accurate data
    additions -- Natfoot
-   I saw the OSM user "Kolossos" at a conference. He presented a budget
    lidar for crowdsourcing 3-D data at his booth. But I think it's only
    suitable for small buildings not for skyscrapers.   (I would like to
    see this talk -- Natfoot +1)
-   We may be able to use Mapillary to get building height. -- Natfoot
-   Just my opinion, but it'd be really nice to see how ortophotos
    improve that... Guys thanks for paying so much attention, learning a
    lot.

