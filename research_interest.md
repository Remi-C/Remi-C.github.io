---
layout: page
title: Research interest
subtitle: A short description of my research interests
---

I'm quite curious and have wide spanning intellectual interests. As such it is no surprise that 
I touched lots of [research subjects](../publi) during my education, [my hobbies](../design_philosophy) and during my working life (such as [consulting and training](../consulting_and_training), see my [CV/Resume](../CV) and [skills](../skills) for more details).

I'd say that the common points are that I like *tangible/graphical* subjects,
and that I put great importancy on *data*.


## Reconstruction
[My PhD]({{ site.baseurl }}{% post_url 2016-09-12-Inverse_procedural_street_modelling %}) is about street reconstruction, so of course I'm interested in reconstruction.

I'm interested in all kind of reconstruction
 - very data-driven ( surface reconstruction from point cloud for instance)
 - model driven (fitting planes, gaussian, etc.)
 - based on procedural/grammar, although there are few articles
 - based on catalog matching (fitting known 3D models from a catalog)

The 3D is to be reconstructed, but sometime it is much more (4D, semantic, network..), which is exciting.

## Modelling
I chose to tackle my [PhD]({{ site.baseurl }}{% post_url 2016-09-12-Inverse_procedural_street_modelling %}) problem with inverse procedural modelling, which implied reading a lot of modelling papers.

I'm really fascinated by modelling, as I see it as a way to abstract (summarize) things.
There is beauty in finding the essence of something.

In my opinion finding a good model is as usefull for a problem as it is usefull for us human to learn something about the things being modelled. 

Of course there are tradeoffs between the chosen model expressivity and its complexity.
At one end the way points are modelled in the [Point Cloud Server]({{ site.baseurl }}{% post_url 2016-02-01-point_cloud_server %}) for instance is very simple, but does not provide much information. At the other end grammar or procedural modelling can generate powerfull models at the price of complexity.

## Remote sensing
I worked 3 years in the french mapping agency using mobile mapping data. 
I really like remote sensing, as this research field mixes massive amount of data and a no-bullshit approach.
Wathever the proposed method, it must really work, not just enough to write a paper about it.

Furthermore, remote sensing research tend to be really close to the hardware used (Lidar, camera, GPS, etc.),
which make the field deeply rooted in engeenering and physics.
The field is also subject to a never ending quest for precision to accurately describe the reality,
which I found challenging.

## Database
Both my work on [street modelling]({{ site.baseurl }}{% post_url 2016-01-01-streetgen %}), on [point clouds]({{ site.baseurl }}{% post_url 2016-02-01-point_cloud_server %}) and on [historical geocoding]({{ site.baseurl }}{% post_url 2017-01-01-historical_geocoding %}) use massively a relational database management system.
I find this field extremely interesting, as the whole system (postgres +postgis + SQL) has been developped for decades to become perfectly adapted to data manipulation.
I found the open source community extremely helpfull and pleasant to work with (both by mail and at sprint).
Besides, PostgreSQL must be the best software I know.

Database presents lots of challenge, of course regarding architecture (cf modelling)
, query optimisation
but also regarding perfomance, indexing, etc.

## Big data / scaling
I faced very soon big data issue regarding [point cloud management]({{ site.baseurl }}{% post_url 2016-02-01-point_cloud_server %}).
Simple, trivial tasks (reading, writing, storing, processing, visualising) become extremely hard when the ammount of data is massive.
Besides an interesting sobering effect about precariousness of computer science, this leads to serious challenges.
I tried both scaling approaches (parallelising and distributing).
At the heart of scaling is the indexing system, and that is another interesting topic,
as indexing is in spirit very similar to compressing, which is dimension reduction (aka clustering).

## Digital Humanities
My thesis superviser works often in the Digital Humanities, and I had the chance to work as a [postdoc]({{ site.baseurl }}{% post_url 2017-01-01-historical_geocoding %}) in the field.
I really like this research domain, because of the end goal, which is to have better understanding of historical processes,
and because of the data, which is a neightmare for computers, because it is so fuzzy!
Everything is fuzzy, the text may have been mispelled, misread, (etc.). 
The temporal aspect is highly fuzzy because we can't be sure of the precise time associated to documents/facts the documents are describing. 
The spatial aspect is also fuzzy, because historical maps may have mistake, wrong georeferencing, etc.

## Image processing and machine learning
I chose image processing (and computer graphics + UX) in engeenering school.
This research domain is at the same time funny (sometimes is feels like trying to make a recipe for cooking) and deeply rooted in mathematics and human perception.
The variety of data of image type is also interesting, especially since the 3D+Z data became so available (kinect).
I worked on machine learning for a working paper (massive point cloud classification).
Machine learning is currently extremely trending (not always for the good reasons).
There is something very satisfaying in finding the appropriate way to model the problem,
then use machine learning to solve it. 
Of course machine learning is a lot about before and after actual machine learning (preprocessing, modelling, dataset, then post processing, tuning, interpreting results, etc)! 

## Robotics
Robotics and mobile mapping research fields have a lot in common.
Both pay attention to hardware, are directed toward robust and working solution, and are interested in understanding the surroundings, which I likes.
Robotics is also abount making decision, triggering actions, and more recently Artificial inteligence, although I'm less familiar with these.
Recently the community has been developping an interesting tool (ROS) that I'd like to work with.


## Smart vehicle 
I spent most of my [PhD]({{ site.baseurl }}{% post_url 2016-09-12-Inverse_procedural_street_modelling %}) time to reconstruct streets and roads with a precision of 10cm.
Besides the road, I also  used reconstruction methods for markings, street furnitures (traffic light, traffic signs, etc.).
The connexion with autonomous vehicle is obvious.
Indeed, autonomous vehciles main problems are understanding the surroundings, and taking decisions about it.
Both these problemes are greatly simplified with a precise and up to date street model !


## Digital fabrication
I have a strong interest in digital fabrication. 
The tools (3D printer, laser cutter, CNC) are not new,what is new is their availability and low price.
These tools seems to have great potential, especially when they'll start to use compter vision/graphics methods to work more robustly, more precisely, and in non-controlled environments.
I'm also interested in those from a design point of view.

In my opinion, the digital fabrication represents an opportunity not for direct product manufacturing, 
but to create templates and helpers to facilitate manufacturing.

## Procedural furniture / guided design
I read several papers about guided design and procedural furniture modelling.
I found these extremely interesting, as a way to simplify access to design, and increase the quality of designed objects.
For instance having a design software that checks in real time that the objects is mechanically sound, or that it can be assembled/disassembled.
From a research perspective, these are extremely challenging, mixing real time simulation and optimisation and visualisation, 
and high level modelling!
Of course this is connected to my interest for [design](../design_philosophy), [design projects](../design_projects) and [woodworking](../woodworking_projects).
