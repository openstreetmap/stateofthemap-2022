---
doi: "10.5281/zenodo.7004634"
layout: session_academic
title: "Floor plan extraction from digital building models"
code: "ZUXTN8"
speaker_names: ['Helga Tauscher']
affiliations: None
room: "Auditorium B"
length: "5"
time: "Sunday, 14:05"
time_iso: "2022-08-21T12:05:00Z"
resources: []
recording: True
---

As part of a larger endeavour to make floor plan representations from building models available for indoor map and navigation services, we study the integration of  IFC and OSM.

<hr>

# Introduction, background, motivation

Official geo data is increasingly published not only in the form of 2D maps,
but also in 3D, mainly as city models in CityGML. Usually the outer shell of
buildings is captured in such models, but they may also involve more intricate
detail. Even more detailed building models are generated during the planning
process for new buildings and renovations. These are nowadays produced in
digital form, archived in as-built phase by owners and operators for the life
time of a building and, in the future, may even be required to be submitted for
building permits.

At the same time there is an increasing public interest in detailed information
about public and semi-public interior spaces, for example about their
accessibility, localization of barriers or targets (e.g. contact persons in
public administration, shops in malls, booths on fairs, markets or larger info
events, departments or hospital wards) or resources (e.g. books in libraries,
charging stations, fire equipment or defibrillators) or to get a first
impression in advance (e.g. virtual open day). The interest and the points of
interest may be temporary or permanent.

Since the context of creating and capturing geo data and building data is
fundamentally different, there is hardly any integration. Indoor data for maps
and navigation models is manually captured or at best derived in undocumented
multi-step semi-automatic workflows.


# Aim and purpose of the study

The project &#34;Level Out&#34; sets out to develop automated methods and services to
make detailed indoor data from digital building models selectively available
for the population of city models, map and navigation services  (in the form of
2,5 D floorplans).

Towards this end, we are developing a platform to check building models whether
they are suitable and contain required data, extract selected and simplified
indoor data and convert it into various formats: CityGML LOD0 (Indoor),
IndoorGML and OSM Indoor.  As input we rely on data in the format IFC (Industry
Foundation Classes), the most widespread standard format for digital building
models.  Indoor OSM, in particular geometry with Simple Indoor Tagging, is one
of the various extraction targets. The data created may not be directly fed
into OpenStreetMap, but serve as a viable base for further mapping.

There are already older solutions, e.g. BIMServerOsmSerializer
(&lt;https://github.com/BIMDataHub/BIMServerOsmSerializer&gt;), which are only built
for a version of IFC, which has been a long time standard version, but
currently approaches towards its end of life: IFC2x3.  There are also solutions
under active development, e.g. the JOSM plugin &#34;Indoor Helper&#34;
(&lt;https://wiki.openstreetmap.org/wiki/JOSM/Plugins/indoorhelper&gt;), which,
however, lack some general approach on the IFC side and coverage of the
heterogeneous options to represent geometry in the IFC schema.  With this
research and development we aim to provide a workflow and software to
systematically access floorplan data in IFC.


# Methodology

We start from both ends of integration by looking at the detailed structures of
the source and target models in parallel.

From the group of target models, we derive a common model, which will have, at
best, near-trivial mappings to OSM Indoor, CityGML, IndoorGML. Although not
strictly necessary for the IFC-to-OSM conversion case or any other bilateral
integration, the intermediate model will not only allow to tackle integration
of IFC with multiple targets besides OSM, but also integration of OSM with
multiple sources besides IFC.

Next, we identify relevant information in the source model. IFC exposes a wide
variety of geometry modelling constructions from CAD software, mainly following
the modelling paradigm of constructive solid geometry (CSG). So far, we found
the following principle representation options:

a) Direct floorplan representation in 2.5D: Here we have 2D representations
   located in 3D space, usually located at the level of the floor finish for a
   particular storey. There are two versions to be distinguished: space
   boundaries versus abstract representations of space-defining elements.

b) Extraction from CSG: Spaces (as well as constructive elements) are often
   represented as solids resulting from extrusion of a planar shape. If extruded
   in z-direction, the base shape can be extracted and used as 2.5-D
   representation.

c) Projection onto floor level: If the geometry is not in CSG-form with
   extrusions, but in BREP (boundary representation), then projection followed by
   a simplification of the projection result is a possible way to extract.

In addition to the geometric elements, there are semantic elements connected to
the geometry that are connected themselves and can be used to charge the
geometric model elements with meaning. Depending on the geometry extraction
method, correlation and consideration of semantic elements is more evident or
complicated - hence possible to different degrees. The paper will discuss these
implications.

After identification of the relevant entities, we are developing a three stage
process for the actual population of target models from IFC.

1. Building model enrichment: Information that can be represented in IFC will
   be played back to the building model instead of being promoted to the generic
   model only.
2. Building to intermedite model: This essential step is coved with a flexible
   rule-based mapping.
3. Intermediate model to target models: Following a careful design of the
   generic model, this step should be simple.

We are testing the processes with data from public buildings, two sets of
university campus buildings as well as one newly built municipal administration
centre. From assessment of the original building data, we will also develop
modelling and export guidelines for BIM software. As far as possible, the demo
data will be made available publicly as open data. More important, the
conversion procedures will be published open source and a respective conversion
service will be offered online.


# Discussion

In summary, our work provides practical benefit in terms of tools to support
the mapping process as well as a scientific contribution in terms of spatial
data integration and expert involvement via domain-specific languages.

The practical benefit of the conversion seems obvious: Building owners can
publish data of their publicly accessible spaces to help with volunteer mapping
work. In the future we will also tackle update, checking and comparison with
existing OSM indoor data.

Scientific contributions are also made in different ways: First, an application
scenario for the OGC Indoor Feature Model is provided and - interesting for the
audience of this conference - evaluation of how OSM data fits with the
generalized model. Further, we explore methods for flexible data integration
with domain specialist and expert community involvement. Finally, but beyond
the scope of this conference, the applicability of integration methods for
bidirectional integration with  multiple sources and targets via intermediary
formats is evaluated.

