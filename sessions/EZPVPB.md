---
layout: session
title: "Corporate editing and its impact on network navigability within OpenStreetMap"
code: "EZPVPB"
speaker_names: [
  'Corey Dickinson (Mcgill University, Geography)',
  'Jugal Patel (Mcgill University, Geography)',
  'Dipto Sarkar (Carlton University, Geography)'
]
affiliations: None
room: "Auditorium B - A101"
length: "5"
time: "Sunday, 10:45"
time_iso: "2022-08-21T08:45:00Z"
resources: []
recording: True
---

Using intrinsic quality indicators we explore how network quality, in terms of its suitability for navigation, varies across areas with relatively high and low corporate editing in OpenSteetMap. Our work shows areas with relatively high rates of corporate editing exhibit not only an overall increase in data quality, but also increased rates at which quality improves.

<hr>

OSM (OSM) contributors have traditionally lacked explicit monetary incentives for contribution [1].  Since 2016, a handful of large corporations (including Apple, Facebook, Microsoft, and Uber) have increasingly contributed data to OSM. Corporate editors (CEs) represent a distinct community as their editors are compensated and thus their contributions cannot be labeled as ‘volunteered’. Additionally, corporations employ large editing teams and new state-of-the-art editing techniques aided by artificial intelligence, making them capable of editing large swaths of information in relatively short time [2]. Corporate teams are often led by long-time OSM community members themselves, emphasizing the multifaceted nature of a rapidly growing open mapping platform [3]. While there has been some contention about the quality of edits done by CEs, corporations argue their contributions improve existing data [7]. Our study provides a preliminary quantitative evaluation of data quality impacts of corporate edits  on OSM.

We assess intrinsic data quality across five regions that have high levels of corporate contributions: Dallas-Ft. Worth, Egypt, Jamaica, Thailand, and Singapore. The quality of these regions is compared to that of Denmark, a region which has witnessed relatively less corporate interest, yet possesses a well-mapped OSM presence due to a well developed local mapping community [4]. These evaluations were performed using measures of intrinsic map quality. While the most straightforward evaluation methods involve comparing against extrinsic sources, such as either ground reference information or authoritative data sources; lack of data availability, licensing terms, and costs often render this comparison untenable [5,6,7]. A transferrable, data driven way of assessing quality remains using Intrinsic Quality Indicators (IQIs), a sub-field of OSM analysis which provides a variety of approaches for evaluating intrinsic OSM data quality. We chose to focus on IQIs that apply to networks, and to evaluate IQIs for land-based transportation networks within OSM. We analyzed networks for our specified locations for every other year between 2014 and 2022.

OSM editing archives were processed using R to extract maps of the relative activity of corporate editors [8]. Our list of corporate editors was sourced from OSM’s publicly available list of corporate editors accounts. We extracted entire networks that represented the first day of each year of interest (2014, 2016, 2018, 2020, 2022) from OSM’s historical archives. For the purposes of this study, we extracted all networks where “OSM WAY = Highway”.

We evaluated several IQIs for our areas of interest.  We focused on completeness of network, both in terms growth over time and in terms of its navigability. We operationalized “completeness for navigability” as an intrinsic measurement by exploring the percentages of networks that possessed attributes necessary for GPS navigation – street names and speed limits. Navigability was assessed and compared across time points using Origin-Destination matrices. By creating a regular matrix across the area and calculating the ratio between a direct route between points, and a route navigated within our network, we calculated a ratio that can be compared across time to evaluate the changing efficiency of the navigable network. Additionally, when building routing networks, we discovered an additional IQI : the presence and qualities of topological islands within our network. That is, areas which are disconnected from the main network due to mapping errors or incompleteness. 

After mapping these metrics, we analyzed how they correlate with each other and how they change over time. Overall, IQI trends for the road network reveal consistent patterns across all measures and locations. There is a trend towards increasing data quality in terms of gradual increase of network length, completeness in terms of attributes (name, speed limit, and pedestrian access), the increasing efficiency of ODM routing ratios, and the increasing amount of places that have “navigable” attributes. Importantly, we found differences between our control location (Denmark) and our other areas of interest. The primary difference of note is not with regards to the quality of the data, but with respect to the rate at which data quality improves: Denmark’s rate of quality improvement is slower than other locations. The faster rate of quality improvement in the test areas highlights that the data creation and editing activity by corporate editors and other organized editors in these locations are helping narrow gaps in data quality.

While this presentation highlights the trends of data quality increase, it does not tease apart the quality assessment of contributions by corporate teams versus other mapping groups. As a crowdsourcing platform, data in OSM is co-produced by repeated editing of data objects by different members of the community [9]. The appearance of CEs in OSM represents the arrival of another community of ‘produsers’ in the OSM ecosystem, and thus a new evolution in its overall trajectory [2,10,11]. Consequently, there is significant interaction between CEs and non-CEs in data co-production in OSM, further reinforcing the idea that OSM is a ‘community of communities’ [11]. Each location has their own patterns regarding editing communities, what they edit, and the sociopolitical and economic ground truth in the real world.  Each of these factors impact the data, and may make comparing editing patterns difficult, especially given the diversity of motivations both with CE communities and within other OSM communities. Hence, we do not try to pry apart the differences in trends between individual countries. Instead, we focus on the overall trend between our test and control locations. With these caveats, we find that the quality of the network has increased in these areas across all tracked metrics at a faster rate than it has in areas with low rates of corporate edits, indicating that corporate editing may have a positive effect on the overall quality of the map.

<hr>

1. Budhathoki, N.R.; Haythornthwaite, C. (2013) Motivation for Open Collaboration. Am. Behav. Sci. 57, 548–575, doi:10.1177/0002764212469364.
2. Anderson, J.; Sarkar, D.; Palen, L. (2019) Corporate Editors in the Evolving Landscape of OpenStreetMap. ISPRS Int. J. Geo-Inf. 8, 232, doi:10.3390/ijgi8050232.
3. Dickinson, C. (2021) Inside the ‘Wikipedia of Maps,’ Tensions Grow Over Corporate Influence. Bloomberg.com.
4. Coast, S. (2015) The Book of OSM; CreateSpace Independent Publishing Platform: California, United States of America; ISBN 1-5142-3274-X.
5. Barron, C.; Neis, P.; Zipf, A. (2014) A Comprehensive Framework for Intrinsic OpenStreetMap Quality Analysis. Trans. GIS 18, 877–895, doi:10.1111/tgis.12073.
6. Senaratne, H.; Mobasheri, A.; Ali, A.L.; Capineri, C.; Haklay, M. (2017) A Review of Volunteered Geographic Information Quality Assessment Methods. Int. J. Geogr. Inf. Sci. 31, 139–167, doi:10.1080/13658816.2016.1189556.
7. Antoniou, V.; Skopeliti, A. (2015) MEASURES AND INDICATORS OF VGI QUALITY: AN OVERVIEW. ISPRS Ann. Photogramm. Remote Sens. Spat. Inf. Sci. II-3/W5, 345–351, doi:10.5194/isprsannals-II-3-W5-345-2015.
8. R Core Team (2022) R: A language and environment for statistical computing. R Foundation for Statistical Computing, Vienna, Austria. URL https://www.R-project.org/
9. Mooney, P.; Corcoran, P. (2014) Analysis of Interaction and Co-Editing Patterns amongst Openstreetmap Contributors. Trans. GIS 18, 633–659, doi:10.1111/tgis.12051.
10. Coleman, D.J.; Georgiadou, Y.; Labonte, J.; Observation, E.; Canada, N.R. (2009)Volunteered Geographic Information : The Nature and Motivation of Produsers. Int. J. Spat. Data Infrastruct. Res. 4, 332–358, doi:10.2902/1725-0463.2009.04.art16.
11.  Solis, P. (2017) Building Mappers Not Just Maps: Challenges and Opportunities from YouthMappers on Scaling up the Crowd in Crowd-Sourced Open Mapping for Development. In Proceedings of the Annual Meeting of the Association of American Geographers; Boston, Massachusetts.

