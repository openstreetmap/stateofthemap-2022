---
layout: session
title: "The cell size issue in OpenStreetMap data quality parameter analyses: an interpolation-based approach"
code: "9HBH3X"
speaker_names: [
  'Silvana Philippi Camboim (UFPR)',
  'Caio Dos Anjos Paiva (UFPR)',
  'Marcio Augusto Reolon Schmidt (UFPR)',
  'Elias Nasr Naim Elias (UFPR)',
  'Everton Bortolini (UFPR)',
  'Guilherme Silva Neivas (UFPR)'
]
affiliations: None
room: "Auditorium B - A101"
length: "5"
time: "Sunday, 10:30"
time_iso: "2022-08-21T08:30:00Z"
resources: []
recording: True
---

The quality of OSM data is dependent on many different factors and is quite heterogeneous. Therefore, in both intrinsic and extrinsic quality parameter analyses, a common practice is subdividing the study areas into subareas. In this paper, we worked on a method for obtaining the optimal grid cell size for OSM data quality analysis. Furthermore, we proposed that if the quality is homogeneous in a region, it can be estimated using an IDW interpolation. . In this summary, we have done a preliminary analysis for a Brazilian city, Curitiba, with about 28,000 points of known accuracy.

<hr>

Knowing the quality of a given geospatial data allows measuring how much its use can be viable in specific applications and assist in decision making. ISO 19157 [1] established that the geospatial data quality indicators are positional accuracy, temporal accuracy, thematic accuracy, logical consistency, and completeness. These measures are represented by values that summarize the condition of a product as a whole. These values tend to be homogeneous throughout the evaluated area in traditional mapping. In contrast, in VGI, data quality can be affected by several conditions related to editing history, contribution period, and contributor profiles [8,9]. Given the mentioned aspects, data quality in VGI platforms tends to be heterogeneous, i.e., the results may show significant discrepancies according to the area assessed or even within the same region.

Given the heterogeneity issues described, several researchers around the world have performed the quality assessment of these types of information based on the principle of subdividing the study area into cells [2,3,4,5,6,7]. Such a procedure has been used in extrinsic quality assessment processes based on ISO 19157 indicators or intrinsic parameters associated with the characteristics of the contributions and contributors. Given the results obtained, the representation of the quality of the data from sub-areas makes it possible to obtain analyses regarding the existence of patterns and establish relationships with other agents and their predominance. The discretization of space into rectangular or hexagonal grids is central to this type of analysis.

The subdivision can occur regularly or irregularly. The units with irregular dimension cells allow us to perform analyses accepting other features or spatial phenomena that define these dimensions (e.g., neighbourhood border, a river or a railway track, areas with different population densities, and the dichotomy between rural and urban areas). However, these methods make operations difficult because they demand that the area value weigh the values; and the spatial analysis considering the neighbourhood is more complex. Units with regular-sized cells solve these two limitations. However, the problem of the grid of cells not conforming to spatial phenomena or features reappears. In order to conform to them, it is necessary to determine the optimal size of the cells.

However, one issue remains little discussed: how to determine the size of such cells. Using too large a cell would treat unequal areas equally. On the other hand, using too small a cell and the increased computational cost of the process, ultimately, the ability to generalize the results is lost. Therefore, in this work, we seek to develop an interactive approach for determining the grid cell size calculation, initially using points of known positional accuracy. The hypothesis here is that when the analyzed subarea is of optimal size, one can interpolate the error within the cell via an IDW and generate minimal residuals at the control points. Furthermore, by consecutively subdividing the grid, the mean squared error versus cell size curve will approach stability, thus revealing the optimal size for a given region.

Inverse distance weighted interpolation (IDW) calculates cell values using sample point sets. This method considers that the higher weights in the interpolation should be due to the proximity of the unknown value point. Thus, if we had a homogeneous behaviour of the quality parameter in an individual area, by interpolation, we could estimate the quality of the points where this value was unknown.

The methodological procedures developed using python in the QGIS environment are:

1. For the study area, points of known positional accuracy are chosen (in our case, intersections of the road system), from which a random subset of 10% is separated as a control set.

2. Definition of a first grid.

3. The points are used for interpolation within each cell by the IDW method. The Root-mean-square deviation (RMSE) is calculated using the control points for each cell and the average of the RMSEs for the entire area;

4. Definition of a second grid with half the resolution of the first grid;

5. Repeat the process described in item 3 for the second grid;

6. Calculate the differences between the average error values of the second grid and the first grid and check their significance ;

7. Repetition of the process described in case there are still values indicated as significant.

In a first analysis, we did a preliminary study for a Brazilian city, Curitiba, with about 28 thousand points of known accuracy. We separated 2.8 thousand control points, and the city was divided into 8 km to 250 m cells. From the preliminary study performed, it was noted that the method show promise in obtaining the necessary analyses to identify the aspects proposed in this work. Furthermore, it was noticed that, as the cell size decreased, the results tended to be more constant, which corroborates the hypothesis of this relationship with data quality. The next steps are to continue the analyses, starting with the verifications and the representation of the magnitude of the differences between different cell sizes.

Although it is a method that still has a relatively high computational cost to be realized, the results are exciting and can be optimized. It is assumed that if it is possible to identify the minimum cell size in which it is possible to estimate the quality of the features, this will help in decision making regarding the incorporation of procedures in different áreas. This method may need even smaller clippings in regions with very heterogeneous characteristics concerning their surroundings (e.g., slums). It is an initial approach to resolve with data a fundamental issue arising from the lack of knowledge of the granularity of discrepancies for each study area.

<hr>

[1] ISO (2013). ISO 19157: 2013 Geographic Information – Data quality

[2] Haklay, M., Basiouka, S., Antoniou, V., &amp; Ather, A. (2010). How many volunteers does it take to map an area well? The validity of Linus’ law to volunteered geographic information. The cartographic journal, 47(4), 315-322.

[3] Fan, H., Zipf, A., Fu, Q., &amp; Neis, P. (2014). Quality assessment for building footprints data on OpenStreetMap. International Journal of Geographical Information Science, 28(4), 700-719.

[4] Martini, A., Kuper, P. V., &amp; Breunig, M. (2019). Database-supported change analysis and quality evaluation of OpenStreetMap Data. ISPRS Annals of the Photogrammetry, Remote Sensing and Spatial Information Sciences, 4, 535-541.

[5] Brovelli, M. A., &amp; Zamboni, G. (2018). A new method for the assessment of spatial accuracy and completeness of OpenStreetMap building footprints. ISPRS International Journal of Geo-Information, 7(8), 289.

[6] Zhang, H., &amp; Malczewski, J. (2017). Accuracy evaluation of the Canadian OpenStreetMap road networks. International Journal of Geospatial and Environmental Research, 5(2).[7] Brovelli, Maria Antonia, Marco Minghini, and Monia Elisa Molinari. “An automated GRASS-based procedure to assess the geometrical accuracy of the OpenStreetMap Paris road network.” (2016): 919-925.

[8] Barron, C., Neis, P., &amp; Zipf, A. (2014). A comprehensive framework for intrinsic OpenStreetMap quality analysis. Transactions in GIS, 18(6), 877-895.

[9] Minghini, M., &amp; Frassinelli, F. (2019). OpenStreetMap history for intrinsic quality assessment: Is OSM up-to-date?. Open Geospatial Data, Software and Standards, 4(1), 1-17.

