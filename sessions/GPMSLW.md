---
doi: "10.5281/zenodo.7004534"
layout: session_academic
title: "Inequalities in the completeness of OpenStreetMap buildings in urban centers"
code: "GPMSLW"
speaker_names: ['Benjamin Herfort']
affiliations: None
room: "Auditorium B"
length: "5"
time: "Sunday, 10:35"
time_iso: "2022-08-21T08:35:00Z"
resources: [{ description: "SOTM_2022_Herfort_lightning_talk", url: "/attachments/GPMSLW_SOTM_2022_Inequalities_xTVAics.pdf" }]
recording: True
---

Albeit the manifold usage of OSM building footprints an adequate investigation into their completeness on the global scale has not been conducted so far. This talk investigates OSM building completeness within all 13,135 urban centers covering about 50% of the global population.

<hr>

The collaborative maps of OpenStreetMap (OSM) have become a major source of geospatial baseline data for humanitarian organisations, companies and public authorities. Describing the elements of spatial data quality (e.g. positional accuracy, completeness, temporal quality) for the OSM dataset is a key prerequisite to provide the potential stakeholders with the necessary information to decide on the fitness for use of a data set for their particular application [1]. Without information on spatial data quality there are serious barriers to the adoption and usage of new sources such as OSM.

A large community of researchers has analyzed the quality of OSM data in comparison to authoritative reference data sets, by means of remote sensing and using intrinsic measures [2–4]. It has been acknowledged that the OSM data in general is strongly biased, in part due to a much larger contributor basis in countries in the global North as a consequence of socio-economic inequalities and the digital divide [5, 6]. Albeit the manifold usage of OSM building footprints an adequate investigation into their completeness on the global scale has not been conducted so far. This talk investigates OSM building completeness in regions home to a population of 3.5 billion people (about 50% of the global population). First, we propose a machine learning regression method based on generalized additive models (GAMs) to assess OSM building completeness within all 13,135 urban centers (as defined by the European Commission [7]). The analysis utilizes an extensive collection of open building data from commercial and authoritative sources as training data and builds upon very recent technological advances to utilize OSM full-history data for spatio-temporal data analysis on the global scale [8]. This allow us – for the first time – to present a comprehensive assessment of the evolution of urban OSM building completeness which encompasses all data contributed to OSM since 2008.

For each urban center we calculated the OSM building completeness using the area ratio method which has been applied55 by several other researchers in the context of urban areas [9–11] . Several measures have been adopted to describe the temporal evolution of inequality in urban OSM building mapping on the global scale and per World Bank region. First, we analyzed the share of population living in urban centers with low completeness (&lt;20%) and high completeness (&gt;80%). Gini coefficient has been utilized to derive the degree of evenness of urban OSM building completeness following an approach proposed by Massey &amp; Denton (1988) to study residential segregation 12 . Moran’s I has been selected as a measure of global spatial autocorrelation of urban OSM building completeness. Spatial autocorrelation has been proposed as an explicitly spatial indicator of segregation covering the dimension of clustering [12, 13]. These analyses has been conducted for annual snapshots from 2008-01-01 up until 2022-01-01.

Overall, urban OSM building completeness is estimated at 38% globally. Our results emphasize that although the well-examined Global North - Global South bias in OSM still exists, over the past years mapping has spread substantially across the globe and within regions. The analysis of the spatial clustering of high completeness values and low completeness values disclosed that global spatial inequality in OSM building completeness has sharply increased between 2008 and 2014. This shows that although overall OSM building completeness became more even in the same period, mapping activity in that time favoured cities which were located close to other cities which were mapped already. One might interprete this as a reinforcing effect. Ongoing mapping in one area triggered even more mapping in surrounded areas. At the same time this also indicates that up until 2014 the expansion of OSM mapping to distant and un-mapped regions (likely to be located in the Global South) didn’t happen at a significant scale.

Nevertheless, since 2014 Moran’s I global spatial autocorrelation declined and was measured at 0.55 as of 2022. Combined with the decrease of the Gini coefficient in the same time, this suggests that OSM building completeness has become more even because mapping activity has been expanded to regions which were previously mapped much less. In that regard, OSM building data as of today was much less segregated in terms of both dimensions (evenness and clustering) compared to the state-of-the-map in 2014. This process was to a limited extend positively influenced but humanitarian mapping activity organized through the HOT Tasking manager, but hardly influenced by corporate mapping activity.

We developed a typology of urban centers based on a methodology to quantify intra-urban completeness pattern by means of evenness and spatial clustering. For this we utilized a fine-scale 1x1 km resolution dataset. In total this analysis covered 4,722 urban centers each with a minimum area of 25 square kilometers. Urban centers have been classified into five different types utilizing an agglomerative clustering approach. Our proposed typology of urban centers incorporates the fact that OSM mapping is rarely distributed equal within cities. Similar findings have been reported for Haiti, where densely mapped zones of Port-au-Prince co-exist alongside zones that remain entirely unmapped [14]. Here we provided a method to quantify these pattern and compare across cities.

The results reveal the need to address the remaining stark data inequalities, which could not be turned around so far by humanitarian and corporate organized mapping activities. We conclude with recommendations directed at stakeholders working with OSM data: (1) Multi-scale building completeness measures should be applied before subsequent usage of OSM data to outline the potential negative effect of missing data. (2) Completeness maps should be used in combination with socio-demographic information to guide future mapping activities to ensure that &#34;nobody is left behind&#34; as encouraged by the SDGs.

<hr>

Oort, P. Spatial data quality: from description to application. Ph.D. thesis, Wageningen Universiteit (2006).

Neis, P., Zielstra, D. &amp; Zipf, A. The Street Network Evolution of Crowdsourced Maps: OpenStreetMap in Germany 2007–2011. Futur. Internet 4, 1–21, DOI: 10.3390/fi4010001 (2011).

Barron, C., Neis, P. &amp; Zipf, A. A Comprehensive Framework for Intrinsic OpenStreetMap Quality Analysis. Transactions GIS 18, 877–895, DOI: 10.1111/tgis.12073 (2014). 9605103.

Senaratne, H., Mobasheri, A., Ali, A. L., Capineri, C. &amp; Haklay, M. M. A review of volunteered geographic information quality assessment methods. Int. J. Geogr. Inf. Sci. 8816, 1–29, DOI: 10.1080/13658816.2016.1189556 (2016).

Sui, D., Goodchild, M. &amp; Elwood, S. Volunteered geographic information, the exaflood, and the growing digital divide. In Crowdsourcing Geographic Knowledge: Volunteered Geographic Information (VGI) in Theory and Practice, vol. 9789400745872, 1–12, DOI: 10.1007/978-94-007-4587-2_1 (Springer, 2013).

Neis, P., Zielstra, D. &amp; Zipf, A. Comparison of Volunteered Geographic Information Data Contributions and Community Development for Selected World Regions. Futur. Internet 5, 282–300, DOI: 10.3390/fi5020282 (2013).

Florczyk, A. J. et al. Description of the GHS Urban Centre Database 2015. February (2019).

Raifer, M. et al. OSHDB: a framework for spatio-temporal analysis of OpenStreetMap history data. Open Geospatial Data, Softw. Standards 4, DOI: 10.1186/s40965-019-0061-3 (2019).

Fan, H., Zipf, A., Fu, Q. &amp; Neis, P. Quality assessment for building footprints data on OpenStreetMap. Int. J. Geogr. Inf. Sci. 28, 700–719, DOI: 10.1080/13658816.2013.867495 (2014).

Törnros, T., Dorn, H., Hahmann, S. &amp; Zipf, A. UNCERTAINTIES OF COMPLETENESS MEASURES IN OPENSTREETMAP – A CASE STUDY FOR BUILDINGS IN A MEDIUM-SIZED GERMAN CITY. ISPRS Annals Photogramm. Remote. Sens. Spatial Inf. Sci. II-3/W5, 353–357, DOI: 10.5194/isprsannals-II-3-W5-353-2015 (2015).

Hecht, R., Kunze, C. &amp; Hahmann, S. Measuring Completeness of Building Footprints in OpenStreetMap over Space and Time. ISPRS Int. J. Geo-Information 2, 1066–1091, DOI: 10.3390/ijgi2041066 (2013).

Massey, D. S. &amp; Denton, N. A. The dimensions of residential segregation. Soc. Forces 67, 281–315, DOI: 10.1093/sf/67.2.281 (1988).

Morrill, R. L. On the measure of geographic segregation. Geogr. Res. Forum 11, 25–36 (1991).

Goldblatt, R., Jones, N. &amp; Mannix, J. Assessing OpenStreetMap Completeness for Management of Natural Disaster by Means of Remote Sensing: A Case Study of Three Small Island States (Haiti, Dominica and St. Lucia). Remote. Sens. 12, 118, DOI: 10.3390/rs12010118 (2020).

