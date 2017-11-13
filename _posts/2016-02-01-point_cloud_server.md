---
layout: post
title: Point Cloud Server
subtitle: a server to manage massive point clouds
tags: [research, publications]
category: research
bigimg: /img/re/thesis_graphical_abstract_line.jpg
---
![abstract Point cloud server](/img/re/thesis_graphical_abstract_line.jpg)
The Point CLoud Server was developed to manage the billions and billions of Lidar point clouds that were produced daily by IGN mobile mapping system.
Rather than deal with files, which limit sharing, management of metadata and concurrent editing,
we chose to use a database server to store groups of points (patch).
The system was successfully used for the PhD work and other projects, and is still being actively researched.

## Abstract

![Point Cloud Server graphical abstract](/img/re/PCS.jpg)

** A scalable and multi-purpose point cloud server (PCS) for easier and faster point cloud data management and processing**


In addition to the traditional Geographic Information System (GIS) data such as images
(rasters) and vectors, point cloud data has become more available. It is appreciated for its
precision and true three-Dimensional (3D) nature. However, managing point clouds can
be difficult due to scaling problems and specificities of this data type. Several methods
exist but are usually fairly specialized and solve only one aspect of the management
problem. In this work, we propose a complete and efficient point cloud management
system based on a database server that works on groups of points rather than individual
points. This system is specifically designed to solve all the needs of point cloud users:
fast loading, compressed storage, powerful filtering, easy data access and exporting,
and integrated processing. Moreover, the system fully integrates metadata (like sensor
position) and can conjointly use point clouds with other geospatial data, such as images,
vectors, topology and other point clouds. The system also offers in-base processing
for easy prototyping, parallel processing and scales well. Lastly, the system is built
on open source technologies and generic and common hardware; therefore, it can be
easily extended and customized. We test the system will several billion points from
point clouds from Lidar (aerial and terrestrial) and stereo-vision. We demonstrate >400
million pts=h loading speed, transparent-for-user and greater than 2 to 4:1 compression
ratio, filtering in the approximately 50 ms range, and output of about a million pts=s,
along with classical processing, such as object detection. 

## Download link
The most recent version of the article is composed by the Chap. 2 of the thesis
[Chap2 of the thesis](https://github.com/Remi-C/inverse_procedural_street_modelling)
[Pdf of article](/img/re/Cura_2016_Pointcloud_server_journal.pdf)
[article on researchgate](https://www.researchgate.net/publication/305363715_A_scalable_and_multi-purpose_point_cloud_server_PCS_for_easier_and_faster_point_cloud_data_management_and_processing?ev=srch_pub)
