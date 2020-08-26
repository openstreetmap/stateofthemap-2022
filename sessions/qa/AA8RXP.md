---
layout: qa
title: "Creating an open data ecosystem for reviews of places and more"
code: "AA8RXP"
---

**Add questions here:**


1.  <s>How can you guarantee reliability of data with pseudonymous
    users?</s>
2.  How can I add reviews to my app? Has anyone built an app (next to
    *mangrove.reviews*), or is there a list?
    1.  A: We are chatting with a projects, but no proper integrations
        yet. You can check out <https://castle-map.infs.ch/> which just
        leads you to the current web app after clicking "Review Object"
3.  What existing open-content review systems did you examine, before
    starting this one? Why were they not adequate? (e.g.
    <https://github.com/eloquence/lib.reviews> , osmand place reviews)
4.  Where can I find more information (online) about Open Reviews
    Association?
    1.  A: See the website: <https://open-reviews.net/>
5.  How do you handle the lack of stable unique identifier in OSM? (see
    <https://wiki.openstreetmap.org/wiki/Overpass_API/Permanent_ID)>
    1.  A: We make use of a Geo URI (
        <https://en.wikipedia.org/wiki/Geo_URI_scheme> ) with a
        reconciliation algorithm that looks at proximity of coordinates
        and the place name.
6.  <s>How are disputes and arbitration handled?</s>
7.  <s>How can one contribute/push this?</s> \[answered\]
8.  Does a central Open Review Identity Provider app for Android exist?
    (I don't know how Android account setting integrations work, but if
    it's not a thing already, I'd be excited to at least look into it.)
    1.  A: It does not yet, it would be great to have someone to have a
        look!
9.  Let's say some \[jerk\] writes a review without ever visiting the
    place. On Google and Facebook he site owner is helpless to fight
    back and get it deleted usually (due to FB and Google being just too
    big to get a word in edgewise.) Hope it won't end up this way too.
    (Maybe 6.)
    1.  A: If the review was left by a one-off user then its unlikely
        that it will be treated as reliable by an algorithm. Otherwise
        the place will need to recoup by getting good reviews. The issue
        with these other platforms is that they start removing good
        reviews since they say those are fraudulent (left by the owner),
        which leads to a negative spiral.
10. What type of things are up for review?
    1.  A: Currently places, websites, books and companies. The standard
        can be easily expanded as long as new open unique identifiers
        are found.
11. What about reviews for services? Could be interesting for cities and
    other public services - as well as for all services perhaps.


**Comments**

-   Your Open Reviews work is so important--thanks! Yelp and Google, for
    example, filter and order results based on advertising customers and
    those who pay more.
    -   A: Thanks!
-   very good and important - I often see new users leaving reviews of
    places missunderstanding the notes - so I think this is a very basic
    and important feature that OSM is lacking today
    -   A: Sounds great, do you think it would be relevant to introduce
        this functionality directly into OSM?
-   Now that the OpenPlaceReviews project is indefinitely on hold, it is
    great to see a new project. (That has some benefits over OPR.)
-   Agreed! Working on fully FOSS/Open Data travel assistance software
    this is one of the missing pieces for us, will look into integrating
    this :)
    -   A: Perfect, please get in touch.
-   I'm a CouchSurfing Host... don't count me out. Yup, even non-profit
    indiviuals get reviews. (Hmmm, so one must not consider me "just
    part of the CS website". And somewhat different that an AirBnB
    for-profit host.)
    -   A: Let us know if you can think how it can work well for this
        case! (On a separate note CouchSurfing might be a nice
        integration partner.)
-   Better add a "Owner rebuttal section": "He said my place didn't have
    a hot shower. Nonsense!"
    -   A: Yep, thats the idea with comments.
-   Awesome talk, thanks!
    -   A: Cheers!
-   Don't say e.g., "minimum 50 characters", most users will "balk out."
    -   A: One can even just leave a rating, no text at all :)


**Information about the Open Reviews Association and the tech**:
<https://open-reviews.net/>
**Link to the presentation slides:**
<https://docs.google.com/presentation/d/1PplC89uEekFp6HYmB2N63ueDGdr3rV0oql60NyPTKb0/edit?usp=sharing>


