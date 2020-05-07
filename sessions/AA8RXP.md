---
layout: session
title: "Creating an open data ecosystem for reviews of places and more"
code: "AA8RXP"
speaker_names_with_affiliations: [&#39;Dina Carabas&#39;]
room: "Track 2"
length: "00:20"
time: "Saturday, 16:30"
resources: [{ description: "Ecosystem", url: "/attachments/AA8RXP_Screenshot_2020-03-29_at_15.55.38_oIv435A.png" }]
recording: True
---
// About us

Mangrove is a non-profit initiative to create a public space on the Internet where people can freely share insights with each other and make better decisions based on open data. The project is set up as an Open Collective, and software is developed open-source by volunteers.

Our goal is to create an open data ecosystem for reviews of places, companies, websites, books, and more. We built open-source infrastructure that enables any application or website to integrate a reviews layer, and to benefit from the shared data pool that is created by a combined user base of participating applications.

// About the proposed session

We propose a 20 minute presentation, roughly along the following outline:

(1) How open data reviews can contribute to the OSM ecosystem (5 min)
  - As consumer choice proliferates, people will rely even more on online reviews to inform their decisions. This makes reviews an increasingly valuable source of insight that helps people navigate our complex world. The problem is that hundreds of millions of people are feeding their valuable insights currently into proprietary data silos.
  - Even the most enthusiastic users of OSM-based navigation apps are forced to switch to Google Maps and other proprietary services to see other people&#39;s opinions about a place. Offering an open data reviews layer can increase the competitiveness with proprietary online map services.
  - An open reviews ecosystem can bring new faces and diversity to the OSM community (e.g., people who want to enrich the factual information with their opinions about the places in their neighborhood).
  - A person who writes a review about a place is more likely to add valuable additional data points back to OSM (e.g., opening hours, wheelchair accessibility, other updates), which can increase the number of contributors.
  - Technological contribution to the ecosystem: proposing and developing a more permanent place identifier scheme

(2) Technology and architecture of Mangrove (8 min)
  - Demo UI (https://mangrove.reviews) to let anyone read and write reviews directly in the open dataset
  - Proposed geo identifier scheme
  - Tools for integration:
    - Infrastructure for storing and retrieving reviews
    - Technical standard to ensure interoperability
    - Open-source API and CC-BY-4.0 licensed dataset
  - Set of algorithms that clean and filter the data
  - Public-key cryptography for privacy-preserving user identification

(3) Challenges (2 min)
  - People who make use of reviews have high expectations towards the geocoding services (search functionality)
  - To build this kind of dataset requires to have permanent place identifiers

(4) Call to action (5 min)
  - Join us in developing this new feature to make OSM more competitive to proprietary mapping services
  - What are ways in which we can leverage people leaving reviews to gain more contributions to OSM (opening hours, wheelchair accessibility, type of services a place offers, etc.)
  - Discuss how to go about permanent place identifiers as the basis for building different products and services using OSM data
