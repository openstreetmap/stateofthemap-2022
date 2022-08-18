---
doi: "10.5281/zenodo.7004593"
layout: session_academic
title: "Returning the favor - Leveraging quality insights of OpenStreetMap-based land-use/land-cover multi-label modeling to the community"
code: "EKEZ7R"
speaker_names: [
  'Moritz Schott (Institute of Geography, GIScience, Heidelberg University)',
  'Adina Zell (Faculty of Electrical Engineering and Computer Science, Remote Sensing Image Analysis Group, Technische Universität Berlin)',
  'Sven Lautenbach (Institute of Geography, GIScience, Heidelberg University)',
  'Begüm Demir (Faculty of Electrical Engineering and Computer Science, Remote Sensing Image Analysis Group, Technische Universität Berlin)',
  'Alexander Zipf (Institute of Geography, GIScience, Heidelberg University)'
]
affiliations: None
room: "Auditorium B"
length: "5"
time: "Sunday, 10:50"
time_iso: "2022-08-21T08:50:00Z"
resources: [{ description: "presentation_slides", url: "/attachments/EKEZ7R_2022_08_21_schott_ligh_Bl93pVn.pdf" }]
recording: True
---

The fitness of OSM for multi-label classification is proven. A workflow to enhance OSM-based multi-labels using machine learning is established. The results are provided to the OSM community via the HOT Tasking Manager.

<hr>

# Introduction

Land-use and land-cover (LULC) information in OSM is a challenging topic. On the one hand, this information provides the background for all other data rendered on the central map and is used by applications like https://osmlanduse.org. On the other hand, this information has a difficult position within the OSM ecosystem. LULC information can be quite cumbersome or even difficult to map e.g. due to natural ambiguity. The growing tagging scheme provides a collection of sometimes ambiguous or overlapping tag definitions that are not fully compatible with any official LULC legend definition [1]. Furthermore, the data is highly shaped by national preferences and imports.

This diversity of the LULC data in OSM is a fundamental principle of OSM that enabled the success of the project. Yet, this can create considerable usage barriers or at least caveats for data users unfamiliar with the projects' ecosystem. The remote sensing community for instance has started to use OSM LULC information as labels in their classification models. Frequently, OSM LULC data has thereby been taken at face value without critical reflection. And, while the quality and fitness for purpose of OSM data has been proven in many cases (e.g. [2,3]) these analyses have also unveiled quality variations e.g. between rural and urban regions. The quality of OSM therefore can be assumed to be generally high, but remains unknown for a specific use-case.

The proposed work first assesses the impact of these challenges on a use-case of multi-label remote sensing (RS) image classification and then provides a machine learning (ML) based workflow to overcome and finally mitigate them. Multi-labels are a type of image classification where a satellite image is labeled with multiple containing LULC classes. In the presented study these labels are extracted from OSM and used to train the ML algorithm.


# Methods and Results

The fitness for purpose of OSM for multi-label RS image classification was tested on a Sentinel 2 scene with a resolution of 10m and four bands in south west Germany recorded in June 2021. The area was chosen for its estimated high completeness and low amount of imported data. OSM data was grouped by its tags into the four LULC classes 'forests', 'agricultural areas', 'build-up area' and 'water bodies'. 18 tags that could unequivocally be mapped to these classes were used and small elements below the image resolution or the classes minimal mapping unit were filtered. The chosen scene was then tiled into a 1.22 x 1.22 km grid of 8100 image patches. Zero to four labels were assigned to each patch, based on the OSM LULC elements therein. Evaluation was performed manually on 910 random patches, of which 80% had a correct OSM-based multi-label, thereby proving the assumed high completeness and quality in the region.

The proposed workflow provides a method to enhance this OSM-based RS image multi-label classification and extend it to areas of lower OSM quality and completeness using ML (specifically deep learning (DL)). The main obstacle for ML and especially DL is the required amount of labeled training data. Volunteered geographic information (VGI) like OSM offers a potential solution to this challenge by providing an overabundance of LULC information that is suitable for this purpose if data quality is sufficiently high. The workflow uses the multi-label information extracted from OSM for training and then detects discrepancies between its predictions and OSM.

Using this information and pinpointing the exact location of error within the patches provides valuable OSM data quality information. Apart from facilitating a fast quality estimation for large areas, the workflow can make its findings automatically available to the OSM community in a feedback loop using the HOT Tasking Manager framework. Thereby the valuable service by the OSM community of providing large amounts of free and generally high quality training data is recognised in the form of quality feedback including mapping hints to the OSM community. 

The five workflow stages are: 1) RS data collection and preprocessing, 2) OSM data collection and preprocessing, 3) LULC multi-label modeling, 4) OSM data issue flagging and 5) the community feedback loop. While each step is an atomic use case and application, the combination of all four steps creates a tool that is useful for the RS and the OSM community likewise. The tool is openly available at https://gitlab.gistools.geog.uni-heidelberg.de/giscience/ideal-vgi/osm-multitag under the GNU Affero General Public License v3 including example datasets. Manual input was kept as low as possible while enabling the 'human in the loop' to take full control over all input and output.

The workflow extracts multi-label training data in stages 1) and 2) as described. Stage 3) then trains a DL model to predict multi-labels using solely RS imagery. For demonstration, the model was trained on the described Sentinel 2 scene in Germany. The models' performance was validated on the manually labeled 910 patches where it outperformed OSM in terms of multi-label accuracy by 7%. When additional errors were manually introduced to the training labels to simulate areas of lower OSM quality or completeness, the model maintained an overall prediction accuracy above the noisy training labels. Alternatively, in cases where OSM LULC multi-label accuracy is suspected to be low, pretrained models from comparable regions with higher OSM data quality can be applied, making the workflow widely applicable.

Any patches where the models' multi-label prediction contradicts the OSM-based multi-label are then detected in stage 4). Multi-labels can be incorrect if either a label is missing (omission), meaning data is missing in OSM, or if a label is wrongly assigned, meaning OSM data is falsely mapped within the tile. The data error type and location within the patch is then extracted using explainable AI [4].

The final stage 5) uses these localised potential OSM data errors to create HOT Tasking Manager projects via the public API. These projects provide additional correction hints. Yet, no automatic editing takes place. The community is kept in full control of all mapping actions as a 'human in the loop'.

# Discussion

The high quality but diverse nature of OSM has been proven for the use-case of multi-label RS image classification. The proposed tool provides an automated OSM multi-label extraction, modeling and verification procedure including a return of results to the OSM community. A major challenge of the approach is the tiled view on the data. If OSM assigns correct multi-labels to a patch, more fine grained data issues will not be detected. Yet, this approach allows large scale data assessments, before the topic of more detailed data improvement is tackled. It also allows to run repeated OSM LULC quality and completeness estimations for large areas over time.

Another major benefit is the usage of local OSM data for modeling, thus making regionalised models the standard procedure. This is required for OSM LULC information as regional data structures and communities exist, that need to be preserved. The model can lead to regional homogenisation and data cohesion within these regional communities.

<hr>

[1] Fonte, C., Milcineski, G., Bovelli, M., Patriarca, J., See, L., Antoniou, V., &amp; Minghini, M. (2016). Automated methodology for converting OSM data into a land use/cover map. In 6th International Conference on Cartography &amp; GIS. Albena. 
[2] Jokar Arsanjani, J., Mooney, P., Zipf, A., &amp; Schauss, A. (2015). Quality Assessment of the contributed land use information from openstreetmap versus authoritative datasets. Lecture Notes in Geoinformation and Cartography, 37–58. https://doi.org/10.1007/978-3-319-14280-7_3 
[3] Fonte, C. C., Bastin, L., See, L., Foody, G., &amp; Lupia, F. (2015). Usability of VGI for validation of land cover maps. International Journal of Geographical Information Science, 29(7), 1269–1291. https://doi.org/10.1080/13658816.2015.1018266 
[4] Zhang, X., Wei, Y., Yang, Y., &amp; Wu, F. (2020, June 13). Rethinking Localization Map: Towards Accurate Object Perception with Self-Enhancement Maps. Cornell University arXiv. Retrieved May 20, 2022, from https://arxiv.org/abs/2006.05220v2

