---
doi: "10.5281/zenodo.7004501"
layout: session_academic
title: "Increasing OpenStreetMap Data Accessibility with the Analysis-Ready Daylight Distribution of OpenStreetMap: A Demonstration of Cloud-Based Assessments of Global Building Completeness"
code: "JRN9DN"
speaker_names: [
  'Jennings Anderson (Meta)',
  'Timmera Whaley Omidire (Meta)'
]
affiliations: None
room: "Auditorium B"
length: "20"
time: "Sunday, 09:00"
time_iso: "2022-08-21T07:00:00Z"
resources: [{ description: "Presentation", url: "/attachments/JRN9DN_anderson_omidire_sotm2_UIJNXSN.pdf" }]
recording: True
---

A recent release of new scientific datasets generated from OpenStreetMap exemplifies the need for analysis-ready repositories of OSM data that require minimal pre-processing. We created the  Analysis-Ready Daylight OpenStreetMap Distribution to provide researchers with the opportunity for simple cloud-based SQL queries of nearly 1B OSM features. We demonstrate the capabilities with intrinsic and extrinsic data coverage assessments of OSM buildings globally.

<hr>

Despite being one of the most open and freely available spatial datasets, OpenStreetMap (OSM) data accessibility remains a challenge. Data accessibility measures how easily end-users can access and use a given dataset for their needs [1]. Because OSM data is intended to be rendered as a map or ingested into routing engines, it is often not easily consumable by data analysts. Pre-analysis workflows require OSM data to be downloaded, parsed, and converted into more common formats, which means that novice end-users of OSM may lack the experience to readily access and use OSM data in decision-making.

Incorporating communities into spatial decision-making processes, such as mapping, is important because a). community members are experts on their communities and b). have a larger stake in final solutions which directly impacts their lived-experiences[2]. OSM empowers a variety of communities, including local governments[3], digital humanitarian groups[4], and even student groups [5], to help navigate and understand places of respective importance.

Research by Nirandjan et al. recently lowered barriers to using OSM data as a reference dataset of critical infrastructure [6]. After categorizing and quantifying particular types of OSM features, the authors released the data in formats more common in geospatial analysis, such as GeoTiffs [6]. This article’s popularity (ranked 90th percentile on the publisher’s website) demonstrates the importance of making OSM data—and datasets derived from OSM—more accessible by means of familiar data structures compatible with common tools. If OSM data were more accessible for analysis, could we see it used in more geospatial research and innovation at large [7]?

While many community-maintained tools exist to convert, extract, and download OSM data, each requires domain knowledge of the unique OSM data structure (nodes, ways, and relations). Furthermore, working at the country or planet-scale requires extensive computational resources. To further lower the barriers to entry for OSM data analysis and extraction, we created the Analysis-Ready Daylight OpenStreetMap Distribution (ARD-OSM). ARD-OSM is published on the registry of open data (RODA) on Amazon Web Services (AWS), where it is freely available to anyone [8]. This dataset containing 1B OSM features is optimized for use with Amazon Athena, a serverless interactive query engine on AWS. Additionally, ARD-OSM has  resolved the OSM data format into common geometries such as points, lines, and polygons. Data also includes pre-computed valuable attributes such as length, surface area, quadkeys, and geographic bounding boxes which are stored as additional metadata. To demonstrate the analytical capabilities of this dataset, next, we will perform a global OSM building density assessment.

Building density is a common metric in OSM quality research, often used to assess map coverage and completeness, such as studied by Yeboah et al. [9]. Measuring building density requires counting all of the buildings within a defined unit of spatial analysis. We use zoom-level 11 map tiles to create an analysis grid that encompasses the global built environment in fewer than 1M tiles. Then, we divide the building count by the area of each map tile to obtain the number of buildings mapped per square kilometer.
Since every feature in ARD-OSM includes the zoom-level 15 quadkey of the map tile in which it exists, we can use a SQL GROUP BY expression instead of a geospatial operator for aggregation. Here is the short query used to count the number of buildings in each zoom-level 11 map tile: 

```sql
SELECT 	substr(quadkey, 1, 11) as z11_tile,
	 	count(id) as number_of_buildings
FROM 	analysis_ready_daylight 
WHERE tags[‘building’] IS NOT NULL AND release = ‘v1.12’
GROUP BY substr(quadkey, 1, 11)
```
In May 2022, running in AWS region us-east-1, this query took 15 seconds and cost just USD $0.10. The results of this query show the density of mapped buildings in OSM to be highest in Europe with additional areas of high density where Humanitarian mapping campaigns have been active such as Nepal, South Eastern Asia, and isolated parts of Africa. This is consistent with the findings of Herfort et al. [10].

How should these densities be interpreted? Do denser regions have higher levels of building completeness in which most or all buildings are mapped? Building density is an intrinsic data quality measure, to further contextualize these findings, we need to perform an extrinsic assessment by comparing our results against an external dataset. A recent study confirmed the viability of referencing population data for building density assessment [11]; and Orden et al. demonstrate a three-step methodology using Facebook’s High Resolution Settlement Layer (HRSL) first requiring both vectorization and spatial aggregation to assess building completeness with respect to population in both the Philippines and Madagascar [12].

Because the HRSL is also published via RODA [13], it can be easily joined to our results. Once HRSL data is incorporated to obtain a measure of buildings mapped per square kilometer per person, we find that parts of Europe remain in the top tiers of density with the most buildings mapped per person. Nepal and many parts of South Eastern Asia, however, are no longer in the same top tier of map coverage. While there are many mapped buildings, the higher populations of these regions reveals that there are still many areas where the buildings have yet to be mapped. This yields a generally lower level of completeness overall than initially identified, which remains consistent with the findings in [10]. Additionally, parts of the United States and New Zealand actually appear more complete with areas of lower density coinciding with regions of lower population, yielding a higher measure of map completeness than before. 

This case study cheaply and easily reproduced popular methods for both intrinsic and extrinsic data quality assessments of OSM building coverage without needing to download nor pre-process any OSM data. The analysis was done completely in the cloud on AWS using free and open data in RODA. Additional metadata in ARD-OSM enabled the query to run efficiently and cost-effectively. The same methodology can be applied to investigations of any other object type in OSM from hospitals to ice cream shops. We also recognize that ARD-OSM does not solve the needs of researchers looking to work with OSM history data. Other tools such as the OpenStreetMap History Database are better suited for those types of historical analyses [14].

The release of OSM-based datasets, such as Nirandjan et al. [6], shows a desire for more researchers to  use OSM data. While OSM data is freely and openly available, researchers must take many steps to download, transform, and ingest the data into an analysis workflow. To solve this, we have made ARD-OSM available in RODA. This analysis-ready dataset contains 1B features—nearly every OpenStreetMap object—in common geospatial feature types such as points, lines, and polygons. To additionally aid researchers, features are enriched with additional metadata describing their location and physical attributes such as length or surface area. From a data accessibility perspective, we anticipate ARD-OSM in future research and innovation, curated by a wide range of end-users, to readily integrate OSM data for decision-making processes which bring communities closer together.

<hr>

1. Open Data Charter. (n.d.) Principles. Open Data Charter. https://opendatacharter.net/principles/

2. Keenan, P.B. &amp; Jankowski, P. (2018). Spatial decision support systems: Three decades on. Decision Support Systems, 116(2019), 64-76. https://doi.org/10.1016/j.dss.2018.10.010 

3. Johnson, P.A. (2017) Models of direct editing of government spatial data: challenges and constraints to the acceptance of contributed data, Cartography and Geographic Information Science, 44:2, 128-138, DOI: 10.1080/15230406.2016.1176536

4. Palen, L., Soden, R., Anderson, T.J., &amp; Barrenechea, M. (2015). Success &amp; Scale in a Data-Producing Organization: The Socio-Technical Evolution of OpenStreetMap in Response to Humanitarian Events. In Proceedings of ACM CHI ‘15. 4113-4122.

5. Maidin, M.A.A., Ahmad, F., Abidin, N.I., Suhaili, J., Awang, M., Rahman, M.A.A., Musa, M.K., Hamidon, N., Yusop, F.M., Syazwan, M.M.S., Harun, H., Hamid, N.H.A., &amp; Kamil, N.A. (2021). Design campus map using OpenStreetMap digital software. In Zaini, M.A.A., Jusoh, M., Othman, N. (Eds.), Proceedings of the 3rd International Conference on Separation Technology. Lecture Notes in Mechanical Engineering (113-129). Springer.  DOI:10.1007/978-981-16-0742-4_8

6. Nirandjan, S., Koks, E.E., Ward, P.J. &amp; Aerts, J.C.J.H. (2022). A spatially-explicit harmonized global dataset of critical infrastructure. Sci Data 9(150). DOI:10.1038/s41597-022-01218-4 

7. National Academy of Sciences, National Academy of Engineering and Institute of Medicine Committee on Ensuring the Utility and Integrity of Research Data in a Digital Age (2009). Ensuring the integrity, accessibility, and stewardship of research data in the digital age. National Academies Press.

8. Daylight Map Distribution of OpenStreetMap was accessed on 2022-04-06 from https://registry.opendata.aws/daylight-osm.

9. Yeboah G, Porto de Albuquerque J, Troilo R, Tregonning G, Perera S, Ahmed SAKS, Ajisola M, Alam O, Aujla N, Azam SI, Azeem K, Bakibinga P, Chen Y-F, Choudhury NN, Diggle PJ, Fayehun O, Gill P, Griffiths F, Harris B, Iqbal R, Kabaria C, … Yusuf R. (2021). Analysis of OpenStreetMap Data Quality at Different Stages of a Participatory Mapping Process: Evidence from Slums in Africa and Asia. ISPRS International Journal of Geo-Information. 10(4):265. DOI:10.3390/ijgi10040265

10. Herfort, B., Lautenbach, S., Porto de Albuquerque, J., Anderson, J., &amp; Zipf, A. (2021). The evolution of humanitarian mapping within the OpenStreetMap community. Nature Scientific Reports 11(3037). DOI:10.1038/s41598-021-82404-z

The rest of the bibliography is here: https://docs.google.com/document/d/1bd1fdidmHWPSNw4lFlRbHpMOtQXsn_rJmR5aam7vfAM/edit?usp=sharing

