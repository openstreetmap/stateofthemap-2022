---
layout: session
title: "Earthquakes and OpenStreetMap"
code: "KNU7L3"
speaker_names_with_affiliations: ["Danijel Schorlemmer"]
room: "Track 1"
length: "00:20"
time: "Sunday, 12:15"
time_iso: "2020-07-05T12:15:00Z"
resources: []
recording: True
---
Earthquakes are threatening many regions in the world with constantly increasing risk due to rapid urbanization and industrialization. To improve resilience and preparedness, we need to estimate the risk of earthquakes with the greatest possible detail. For this, exposure models are used that translate the physical earthquake hazard to building damage, human and financial losses. The level of detail in the risk model directly depends on the level of detail in the exposure model. So far, exposure models are usually described as aggregated building-type descriptions for larger geographic areas, from city districts to even larger administrative units.

We present our new open, dynamic, and global exposure model based on OpenStreetMap that does not stop at administrative boundaries but rather attempts to classify and describe every building on Earth with the greatest level of detail. Our open-source model extracts all possible exposure indicators, i.e. footprint shape, number of stories, occupancy type, shape of the roof, etc. and combines the OpenStreetMap data with other open datasets if available. Using these indicators, the model assesses in a probabilistic way the possible building classes, the number of people inside the building depending on the time and day, and the reconstruction value. In areas with incomplete building coverage, the classical aggregate-based exposure models are combined with our model to deliver a probabilistic description of the entire building stock. To achieve a better spatial distribution of buildings in areas of incomplete coverage, we estimate the likely locations of buildings through remote sensing using again open data only, mainly Sentinel-I radar data. Due to the near-realtime computations of our model, it directly profits from the growth of OpenStreetMap and with about 5 million buildings added each month, the areas of incomplete coverage are constantly shrinking, making way for our building-specific exposure model.
