---
doi: "10.5281/zenodo.7004509"
layout: session_academic
title: "OSM for sustainable transport planning"
code: "CEMMTQ"
speaker_names: [
  'Greta Timaite (University of Leeds)',
  'James Hulse (University of Leeds)',
  'Robin Lovelace (University of Leeds)'
]
affiliations: None
room: "Auditorium B"
length: "20"
time: "Sunday, 12:30"
time_iso: "2022-08-21T10:30:00Z"
resources: [{ description: "Academic Track Presentation", url: "/attachments/CEMMTQ_sotm2022_slides_update_HxoiqCX.pdf" }]
recording: True
---

OpenStreetMap (OSM) data has the potential to facilitate bottom-up approach to transport planning which is essential for localized data-driven policy interventions. Given this, OpenInfra project is exploring the potential of OSM data in transport research with a focus on active travel. The exploration showed that currently missing data limits the applicability of OSM data. Nevertheless, we argue that the potential and relevance of OSM data can be demonstrated by recategorizing OSM data to provide more actionable insights to policy-makers. This, therefore, could encourage the uptake of open data leading to more transparent, reproducible, and participatory transport planning.

<hr>

One of the key domains in which OpenSteetMap (OSM) data has been utilized is transport research [1]. OSM has been used in agent-based transport simulation [2] and routing [3], including cycling [4], walking [5], wheeling [6], and blind pedestrian routing [7]. Another application of OSM data is in transport infrastructure planning. Nelson et al. [8] argue that OSM has the potential to become a primary source of data on infrastructure across the globe. 

Regardless of OSM’s potential to become a primary source of data on infrastructure, its potential in active travel infrastructure planning is yet to be realized. One of the potential reasons behind this lag might be linked to the perceived unreliability of open-access crowdsourced data [9]. The quality of OSM has received extensive examination [1] in which the question concerning data completeness plays a significant role because, it is argued, the mappers are not coordinated to guarantee systematic coverage [10]. To address this issue, Barrington-Leigh and Millard-Ball [11] assessed OSM road completeness and found that globally over 80% of roads are mapped. Problematically, however, their assessment focused on roads designed for motor traffic, thus excluding other modes of transport. This gap has been partially addressed by Ferster et al. [12]who examined and compared OSM cycling infrastructure in Canada. They have not, however, considered the infrastructure from the perspective of accessibility. Moreover, there seems to exist no equivalent study using OSM data in the context of pedestrian infrastructure planning. 

Nevertheless, open-access crowdsourced data, such as OSM, can support an increasing need for local evidence to inform transport policies. This is important in the context of the UK in which a shift from provision for motorised modes towards more sustainable active modes of travel, such as walking, wheeling, and cycling, takes place [13]. The importance of localizing interventions to meet the needs of local communities has been outlined in both policy [15] and academic [16] papers. A potential way to engage citizens in the decision-making is to encourage “produsage” – a model in which citizens both produce and use data [17]. 

Acknowledging the potential of OSM to boost citizen participation, OpenInfra project, run at the University of Leeds (UK), aims to address the gap of literature regarding the potential OpenStreetMap in transport research. The project started by examining the existing OSM tags relevant to active travel infrastructure in England with a focus on West Yorkshire, Greater Manchester, Greater London, and Merseyside. The data has been queried using osmextract [18], a package in R, and explored using exploratory data analysis (EDA) approach. A reproducible code containing all the figures discussed here can be found on GitHub: https://github.com/udsleeds/openinfra/tree/main/sotm2022 

Given the extensive use of OSM data in transport research, it is not surprising that OSM provides a comprehensive active travel network, yet there is a lack of specification concerning the type of infrastructure that is present (e.g. is it a cycle lane or a cycle track?). For instance, cycleways and footways constitute about 1/3 of all the mapped highways on which one can legally walk, wheel or cycle but only a few percent of the cycleways and footways have tags detailing their type. The data gets even scarcer in the context of accessible infrastructure planning. For example, there is a lot of missing information on the presence and type of kerbs – a street element that might make the movement of a wheelchair user more challenging [19]. 

The missing data currently limits the use of OSM data in active travel planning, however this does mean that the use of OSM data should be dismissed. Following Nelson et al.’s [8] argument that it is important to make crowdsourced data more actionable, we decided to recategorize OSM data based on Inclusive Mobility (IM) [15], a guide that outlines the best practices in creating inclusive pedestrian infrastructure in the UK. For this, a function has been written (documentation can be found here: https://udsleeds.github.io/openinfra/articles/im_get.html). It takes an OSM dataframe, recategorizes its tags based on the definitions outlined in the guide, and returns an OSM dataframe with new columns to use in further analysis. However, the function provides a simplification of the IM guide for a couple of reasons. The first one could be considered in terms of definitional discrepancies. For instance, the guide defines footways as “pavements adjacent to roads”, yet this is not easily extracted from the OSM in which highway=footway is a generic tag and often there is no further refinement (e.g., sidewalk=*) to determine if it is a pavement adjacent to a road. Another reason is linked to assigned values. For example, the guide identifies six tactile paving surfaces but OSM focuses on the presence/absence of tactile paving, thus limiting how much information can be extracted from the data. 

One potential application of the IM function could be to explore the existence and geographic distribution of accessibility indicators, such as the presence of a flush kerb. Yet, more interesting results can be produced by using recategorised OSM data in conjunction with other datasets that would help to improve the understanding of the accessibility of streets. As an illustration for this, an open-access Leeds Central Council Footfall data was used [20]. We reasoned that the locations at which footfall data were collected are heavily used by pedestrians, thus demonstrating the need to ensure inclusive spaces. 5 unique streets were identified, which resulted in 35 linestrings in OSM. Then, a basic index of accessibility, ranging from 0 to 5, was created. For example, if a linestring is classified as a footway, footpath, or implied footway based on the IM guide, then it received 1, otherwise 0. If a flush kerb is mapped, it received 1, otherwise (e.g., not flush or NA), 0 is given. Finally, the values were added and a final index produced. Following this, the highest index score is 2 (19 linestrings), while the rest scored 1. This example does not necessarily show that the streets are inaccessible because the missing data make it hard to make a fair judgement (e.g., in this case not a single linestring has data on kerbs). However, we would argue that this is a space for OSM to produce more readily actionable insights regarding transport infrastructure, especially if joined with other (open) datasets that would help to overcome some of its current data limitations. 

The following steps of the OpenInfra project are focused on scaling up. The goal is to produce ‘OSM transport infrastructure data packs’ for transport authorities in England to support the uptake of open-access data, such as OSM, in transport planning. We believe that the utilization of open-access data could make transport planning more transparent, reproducible, and participatory which, consequently, would support an uptake of sustainable modes of travel. OSM specifically has the potential to provide localized insights on the existing transport infrastructure and facilitate more inclusive and accessible transport planning.

<hr>

1. Jokar Arsanjani, J., Zipf, A., Mooney, P., &amp; Helbich, M. (2015). An Introduction to OpenStreetMap in Geographic Information Science: Experiences, Research, and Applications. In J. Jokar Arsanjani, A. Zipf, P. Mooney, &amp; M. Helbich (Eds.), OpenStreetMap in GIScience: Experiences, Research, and Applications. Springer International Publishing.  

2. Ziemke, D., Kaddoura, I., &amp; Nagel, K. (2019). The MATSim Open Berlin Scenario: A multimodal agent-based transport simulation scenario based on synthetic demand modeling and open data. Procedia Computer Science, 151, 870–877.  

3. Luxen, D., &amp; Vetter, C. (2011). Real-time routing with OpenStreetMap data. Proceedings of the 19th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems, 513–516.  

4. Yeboah, G., &amp; Alvanides, S. (2015). Route Choice Analysis of Urban Cycling Behaviors Using OpenStreetMap: Evidence from a British Urban Environment. In J. Jokar Arsanjani, A. Zipf, P. Mooney, &amp; M. Helbich (Eds.), OpenStreetMap in GIScience: Experiences, Research, and Applications. Springer International Publishing.  

5. Zielstra, D., &amp; Hochmair, H. H. (2012). Using Free and Proprietary Data to Compare Shortest-Path Lengths for Effective Pedestrian Routing in Street Networks. Transportation Research Record, 2299(1), 41–47.  

6. Neis, P. (2015). Measuring the Reliability of Wheelchair User Route Planning based on Volunteered Geographic Information. Transactions in GIS, 19(2), 188–201.  

7. Cohen, A., &amp; Dalyot, S. (2021). Route planning for blind pedestrians using OpenStreetMap. Environment and Planning B: Urban Analytics and City Science, 48(6), 1511–1526.  

8. Nelson, T., Ferster, C., Laberee, K., Fuller, D., &amp; Winters, M. (2021). Crowdsourced data for bicycling research and practice. Transport Reviews, 41(1), 97–114.  

9. Basiri, A., Haklay, M., Foody, G., &amp; Mooney, P. (2019). Crowdsourced geospatial data quality: Challenges and future directions. International Journal of Geographical Information Science, 33(8), 1588–1593.  

10. Haklay, M. (2010). How Good is Volunteered Geographical Information? A Comparative Studyof OpenStreetMap and Ordnance Survey Datasets. Environment and Planning B: Planning and Design, 37(4), 682–703.  

11. Barrington-Leigh, C., &amp; Millard-Ball, A. (2017). The world’s user-generated road map is more than 80% complete. PLOS ONE, 12(8).  

12. Ferster, C., Fischer, J., Manaugh, K., Nelson, T., &amp; Winters, M. (2020). Using OpenStreetMapto inventory bicycle infrastructure: A comparison with open data from cities. International Journal of Sustainable Transportation, 14(1), 64–73.  

13. BEIS. (2021). Net Zero Strategy: Build Back Greener. 

14. Department for Transport. (2020). Cycle infrastructure design. 

15. Department for Transport. (2021). Inclusive mobility. 

16. Aldred, R., Woodcock, J., &amp; Goodman, A. (2016). Does More Cycling Mean More Diversity in Cycling? Transport Reviews, 36(1), 28–44.  

17. Boularouk, S., Josselin, D., &amp; Altman, E. (2017). Ontology for a voice transcription of OpenStreetMap data: The case of space apprehension by visually impaired persons. World Academy of Science, Engineering and Technology. 

18. Gilardi, A., &amp; Lovelace, R. (2021). Osmextract: Download and Import Open Street Map Data Extracts.  

19. Timaite, G., Lovelace, R., &amp; Houlden, V. (2022). The potential of OpenStreetMap for (accessible) active travel planning. 30th Annual Geographical Information Science Research UK.  

20. Leeds City Council. (2021). Leeds City Council Footfall Camera Aggregated Data. CDRC.

