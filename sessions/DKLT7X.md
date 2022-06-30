---
layout: session
title: "A review of Mapillary-generated map data and how accuracy compares across devices"
code: "DKLT7X"
speaker_names: ['Said Turksever']
affiliations: Meta/Mapillary
room: "Auditorium B - A101"
length: "20"
time: "Friday, 17:00"
time_iso: "2022-08-19T15:00:00Z"
resources: []
recording: True
---

Mapping is time-consuming and requires a high workforce when it comes to keeping maps up-to-date. Mapillary brings a different approach to geospatial data collection with street-level imagery. This approach allows communities to collect geospatial data faster and cheaper. But can Mapillary-generated data be useful for enriching OpenStreetMap? In this study, Mapillary-extracted map data will be examined against ground truth to assess data quality on contributing to OpenStreetMap.

<hr>

In this case study the positional accuracy and completeness are assessed by benchmarking Mapillary-generated data against ground truth for street light provided by Ordu Metropolitan Municipality in the borough of Altinordu, which covers an area of 9 km2. A total number of 323 street lights were recorded in the authoritative dataset.

Completeness and positional accuracies are evaluated for each street light for different camera setups. In order to compare the impact of camera type on positional accuracy, street-level imagery was collected with three different cameras: iPhone 11, GoPro Hero 7 Black and GoPro Max. Collected street-level imagery was uploaded to Mapillary by using the Desktop Uploader. Imagery which are captured from different cameras is isolated during the upload to compare map data accuracy, completeness and correctness comparison based on camera type.

In this experiment, we validate the effectiveness of Mapillary extracted map data by focusing on streetlights by evaluation results based on completeness and positional accuracy key performance indicators. The best result of completeness is achieved with GoPro Hero 7 Black with 87.57% in the working area and it is followed by GoPro MAX with 77.30% for Mapillary extracted street light data . Lastly, the completeness of iPhone 11 acquired data is 71.89%.

In terms of positional accuracy, our experiment shows GoPro MAX captured street-level imagery can be extracted with 2.02 m of positional error and it is followed by GoPro Hero 7 Black with 2.17 m of positional error. The average positional error of street light which is extracted from iPhone 11 captured street-level imagery is 2.21 m. This positional error is close to the precision of a single frequency GPS receiver.

This experimental study shows that positioning accuracy is highly related to the GPS accuracy of the capture device, and in general, a large part of the final positional error can be attributed to this. Mapillary's 3D reconstruction is able to mitigate some of these effects. Additionally, capturing with a large field of view has a positive effect on accuracy. In this study we also validate that positional accuracy depends on various factors of the capture process; precision of GPS receiver and additionally positioning hardware, resolution and quality of the images, image capture frequency of the camera, imagery density in the working area and type of photo such as flat or 360.

The overall positional accuracies are under 5m which can be a promising solution for enriching street lights data on OpenStreetMap and collecting streetlights inventory for the municipalities and governmental bodies if this data will not be used for surveying purposes or reference data, however Mapillary-generated data can be useful and time effective as complementary data with low cost collection expenses.

