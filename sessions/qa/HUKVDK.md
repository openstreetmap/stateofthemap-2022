---
layout: qa
title: "From Historical OpenStreetMap data to customized training samples for geospatial machine learning"
code: "HUKVDK"
---

**DOI**: <https://doi.org/10.5281/zenodo.3923040>
**Github**:  <https://github.com/GIScience/ohsome2label>
**OSM Science Mailing list**:
<https://lists.openstreetmap.org/listinfo/science>


**Questions**

1.  \[Done\] Does ohsome2label also georeference the results (i.e. land
    use vectors, building footprint vectors)?
2.  \[Done\] Question from René: Thanks a lot for your talk! I'm
    wondering how your approach performs in areas with lower OSM data
    quality or with sparser coverage. Have you conducted systematic
    performance tests in corresponding areas? Would be interesting in
    support of your ongoing work in the Global South, in particular.
    Yes, it is :)
3.  \[Done\] How do you ensure the imagery is exactly WGS84 with no skew
    before you start? Bing: bad, Maxar: often bad.-jidanni
    1.  Bing is often up to 10 meters offset in rural areas! Basing work
        on it will really damage the resulting map.
4.  \[Done\] In some works landuse/landcover information have been
    derived from geosocial media data, especially from shared photos. Do
    you see any potential for augmenting your approach taking account
    also of these data sets (in some areas) especially with regards to
    possibly achieving fine temporal resolution? \[\]Do you think this
    could add anything to what you achieve already using OSM data?
5.  \[Done\] Can you discuss more about your future plans for the OSM
    quality measurement? Would be interesting to know!
    1.  Oh no I think it's kind of choppy, I wasn't able to hear.
    2.  I'll just discuss through email later, thanks! Thank you too for
        your participation!
6.  Can you compare your work and the work of Development Seed with
    Label maker? I'm curious to know the similarities and differences.


Answer:

1.  Yes, the result is in slippy map tile format.
2.  It's two question, for sparse coverage area, it works well since
    ohsome API offers a roboust feature query function. For the lower
    quality  area, some more post processing should be done for your
    training dataset.
3.  We support customed tms, you can change the bad image with the
    corresponding image.
4.  The geosocial media data is varies in different application, so it's
    hard to handle it in a unified form. But I will think about it, or
    you can raise an issue on our github page. Thanks! My question was
    rather exploratory in nature, indeed. Hopefully inspirational though
    :)
5.  First, we will try to do some tag-specified intrinsic data
    indicators, like the quality indicator for the building. Second, our
    next step is to study how the tile-based osm data quality influence
    the deep learning training progress.
6.  For the Label maker, if you have used it before. You will find it's
    hard to setup. For ohsome2label, you only need to type \`pip install
    ohsome2label\` then you can get it. The second difference is that we
    support some data quality analysis for your area of interest, and we
    will extend this function further. Third, we use MS coco format
    output and Label marker use npz. Fourth, we have the intermidiate
    output, so you can modified what you want, like add some feature to
    your geojson. Ah, we also support overpass api aside Ohsome API.


Thank you for your great question. You can connect us by email or on our
github page any time. It's our pleasure. My email is
zhaoyan\_wu@whu.edu.cn. Many thanks for taking time to address the
questions; you were excellent!Thank you!

**Comments**

1.  Award winning session chair. Thanks+1. Many thanks! :)+1 Should say
    "I'm XX, talking to you from YY (country)".
2.  audio on video is over blown.+1
    1.  Noted and thanks, video team will have a look.
        1.  (Might be a problem of the recording / microphone rather
            than the stream.)+1
        2.  (had to turn down the audio source as it was too loud
            complared to live source.)

