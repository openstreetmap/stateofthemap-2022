---
layout: session
title: "The Map in 360"
code: "YTHZWC"
speaker_names_with_affiliations: ["Said Turksever"]
room: "Track 1"
length: "00:20"
time: "Saturday, 15:00"
resources: []
recording: True
---
Mobile mapping is the process of collecting geospatial data from a mobile vehicle using a 360º camera, laser scanner, GPS/IMU positioning system, and other sensors. Mobile mapping is a time and cost-effective way to conduct asset inventory, monitor road infrastructure, and map street furniture. However, the high cost of acquiring mobile mapping equipment, such as professional 360° cameras and laser scanners, inhibit the ability of local OpenStreetMap communities to leverage mobile mapping technologies. With advice from Mapillary, low-cost devices that are accessible to communities make mobile mapping possible on a wider scale.

360º cameras may be used in different vehicle types: cars, bicycles, quad bikes and also on foot. With a 360º field of view, these cameras capture everything around the sphere. Where flat frame images can limit the map editing workflow, 360º images bring panoramic viewing to OpenStreetMap editors for a more comprehensive understanding of the space and place. The Mapillary photo overlay supports panorama view on OSM ID Editor and JOSM.

After images have been captured and uploaded to the web, Mapillary creates a reconstruction of the scene in 3D using an open-source Structure from Motion library (OpenSfM). This helps to improve the image GPS positions, based on the overall consistency of the 3D scene. Next, the objects in the imagery (such as traffic signs and other types of objects) are identified by computer vision. Combining detections of an object in several images and the aforementioned 3D model allows us to calculate the position of the detected object in the world. 

Overall, this talk will examine the recommended 360º cameras, discuss data collection and benefit of street-level imagery collection with 360º cameras, review strategies for uploading 360º images, comparing different 360º camera models, and highlight how OpenStreetMap communities around the world are using 360º images to improve local maps with Mapillary.
