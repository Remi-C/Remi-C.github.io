---
layout: post
title: Implicit Level Of Detail for Point Clouds
subtitle: LOD contained in the order of points 
tags: [research, publications]
category: research
bigimg: /img/lod_banner.png
---
![LOD abstract](/img/lod_banner.png)
When we created the Point Cloud Server to manage billions of points, several method processing methods were used on points.


It was rapidely clear that for almost any methods, and for visualization in perticular, a way to reduce the number of points was needed.
Our solution was the Implicit Level of Detail method, where points are ordered by decreasing importancy in each group of points (patch). Then reducing the number of point was a matter of taking only the n first points per patch.
The method was refined, and led to the creation of a robust dimensionnality descriptor, along with its uses for classification and pre-processing.
Initially regrouped in one article, this two topics (LOD and dimensionnality descriptor) were too complex to be handled together, which led to a split into two articles which are much easier to read.



## Abstract
### Implicit Level of Detail for the Point Cloud Server ###
![Implicit LOD grpahical abstract](/img/re/lod_banner_short.png)
Lidar datasets now commonly reach Billions of points and are very dense. Using
these point cloud becomes challenging, as the high number of points is untractabel for
most applications and for visualisation. In this work we propose a new paradigm to
easily get a portable geometric Level Of Details (LOD) inside a Point Cloud Server. The
main idea is to not store the LOD information in an external additional file, but instead
to store it implicitly by exploiting the order of the points. The point cloud is divided
into groups (patches). These patches are ordered so that their order gradually provides
more and more details on the patch. We demonstrate the interest of our method with
several classical uses of LOD, such as visualisation of massive point cloud, algorithm
acceleration, fast density peak detection and correction.

### A new dimensionnality descriptor for patch classification in the Point Cloud Server ###

![Dimensionnality descriptor graphical abstract](/img/re/dim_desc_lod.png)

Lidar datasets are becomming more and more common. They are appreciated for their
precise 3D nature, and have a wide range of applications, such as surface reconstruction,
object detection, visualisation, etc.
For all this applications, having additional semantic information per point has potential
of increasing the quality and the efficiency of the application.
In the last decade the use of Machine Learning and more specifically classification
methods have proved to be successful to create this semantic information. In this paradigm,
the goal is to classify points into a set of given classes (for instance tree, building, ground,
other).
These methods use descriptors (also called feature) of a point to learn and predict its
class.
Designing the descriptors is then the heart of these methods. They can be based on
points geometry and attributes, use contextual information, etc.
In this work we propose a new simple geometric descriptor that gives information
about the implicit local dimensionnality of the point cloud at various scale. For instance
a tree seen from afar is more volumic in nature, yet locally each leaves is rather plannar.
To do so we use an octree centered on the point, and compare the variation of the
occupancy of the cells across the levels.
We compare this descriptor with the state of the art dimensionality descriptor and
show its interest. We further test the descriptor for classification wihtin the Point Cloud
Server (Cura, 2016), and demonstrate efficiency and correct results.


## Download link
The most recent version of the articles are in fact the Apppendix A and B of the thesis.
[Appendix A and B of the thesis](https://github.com/Remi-C/inverse_procedural_street_modelling)


[article not split on arxiv](https://arxiv.org/abs/1602.06920)


[article not split on researchgate](https://www.researchgate.net/publication/296702210_Implicit_LOD_for_Processing_Visualisation_and_Classification_in_Point_Cloud_Servers)
