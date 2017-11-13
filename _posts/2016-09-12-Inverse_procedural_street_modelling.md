---
layout: post
title: Inverse Procedural Street Modelling
subtitle: My PhD thesis about reconstructing street for large cities using procedural methods and point clouds.
tags: [research, publications]
category: research
bigimg: /img/re/general_graphical_abstract_for_defense.jpg
---
![phd abstract](/img/re/general_graphical_abstract_for_defense.jpg)
My PhD was about Inverse procedural street modelling, that is generate a street model (Chap3. road network, geometry, traffic information, street objects), then fit this street model to real life (chap5.). Real life here is expressed by massive point clouds (Chap2, Appendix A and B).
Of course, the fitting is automatic, but nevertheless it is essential to allow the users to perform manual edit of the street model, in a in-base shared and concurrent way (chap 4).

More generally, the PhD is about reconstruction inverse procedural modelling, which led to a very large state of the art about procedural modelling, inverse problems and urban reconstruction in general (chap 1)

## Abstract
![historical geocoding abstract](/img/re/historical_geocoding_abstract.png)

World urban population is growing fast, and so are cities, inducing an urgent need
for city planning and management. Increasing amounts of data are required as cities
are becoming larger, "smarter", and as more related applications necessitate those data
(planning, virtual tourism, traffic simulation, etc.). Data related to cities then become
larger and are integrated into more complex city models.
Roads and streets are an essential part of the city, being the interface between public
and private space, and between urban usages. Modelling streets (or street reconstruction)
is difficult because streets can be very different from each other (in layout, functions,
morphology) and contain widely varying urban features (furniture, markings,
traffic signs), at different scales.
In this thesis, we propose an automatic and semi-automatic framework to model and
reconstruct streets using the inverse procedural modelling paradigm. The main guiding
principle is to generate a procedural generic model and then to adapt it to reality using
observations. In our framework, a "best guess" road model is first generated from very
little information (road axis network and associated attributes), that is available in most
national databases. This road model is then fitted to observations by combining inbase
interactive user edits (using common GIS software as graphical interface) with
semi-automated optimization. The optimization approach adapts the road model so
it fits observations of urban features extracted from diverse sensing data. Both street
generation (StreetGen) and interactions happen in a database server, as well as the
management of large amount of street Lidar data (sensing data) as the observations
using a Point Cloud Server.
We test our methods on the entire city of Paris, whose streets are generated in a few
minutes, can be edited interactively (<0.3 s) to regenerate the street model) by several
concurrent users. Automatic fitting (few min) shows promising results (average distance
to ground truth reduced from 2.0m to 0.5m).
In the future, this method could be mixed with others dedicated to the reconstruction
of buildings, vegetation, etc., so an affordable, precise, and up to date city model can be
obtained quickly and semi-automatically. This will also allow such models to be used
in other application areas. Indeed, the possibility to have common, more generic, city
models is an important challenge given the cost and complexity of their construction.

## Download link
[The thesis manuscript](https://github.com/Remi-C/inverse_procedural_street_modelling)
