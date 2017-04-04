---
layout: post
title: StreetGen
subtitle: an in-base tool for street modelling
bigimg: /img/re/logo_streetgen_HQ.png
tags: [research, publications]
category: research
---

StreetGen is the method that was developped during the PhD to generate a street model including the road, the traffic information, and the street objects.
Everything (base data, method, resulting street model) is contained within a database, which make it scale nicely and allow concurrent interactive editing.

## Abstract

** Procedural modelling of streets**

![StreetGen Graphical abstract](/img/re/streetgen_graphical_abstract.png)

Streets are large, diverse, and used for several (and possibly conflicting) transport
modalities as well as social and cultural activities. Proper planning is essential and requires
data. Manually fabricating data that represent streets (street reconstruction) is
error-prone and time consuming. Automatising street reconstruction is a challenge because
of the diversity, size, and scale of the details (10 cm for cornerstone) required. The
state-of-the-art focuses on roads (no context, no urban features) and is strongly determined
by each application (simulation, visualisation, planning). We propose a unified
framework that works on real Geographic Information System (GIS) data and uses a
strong, yet simple hypothesis when possible to coherently model streets at the city level
or street level. Because it is updated only locally in subsequent computing, the result
can be improved by adapting input data and the parameters of the model. Our street
model is based on street axis, and contains geometric information (road surface, sidewalk),
topological information (street connection), as well as traffic information and 
street objects. We reconstruct the entire Paris streets in a few minutes. We tested the
usefulness of our model for several applications, such as 3D city building and traffic
simulation.


## Download link
[The thesis manuscript, chap.3 ](https://github.com/Remi-C/inverse_procedural_street_modelling)
[the conference paper (very short)](/_collection/Cura_2015_StreetGen.pdf) 
[Link to researchgate](https://www.researchgate.net/publication/283184997_STREETGEN_IN-BASE_PROCEDURAL-BASED_ROAD_GENERATION)
