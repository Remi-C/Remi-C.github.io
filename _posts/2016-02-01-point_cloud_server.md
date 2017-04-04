---
layout: post
title: Point Cloud Server
subtitle: a server to manage massive point clouds
bigimg: /img/PCS.jpg
tags: [research, publications]
category: research
---


## Abstract

![Point Cloud Server graphical abstract](/img/re/PCS.jpg)

In addition to the traditional Geographic Information System (GIS) data such as images
(rasters) and vectors, point cloud data has become more available. It is appreciated for its
precision and true three-Dimensional (3D) nature. However, managing point clouds can
be difficult due to scaling problems and specificities of this data type. Several methods
exist but are usually fairly specialised and solve only one aspect of the management
problem. In this work, we propose a complete and efficient point cloud management
system based on a database server that works on groups of points rather than individual
points. This system is specifically designed to solve all the needs of point cloud users:
fast loading, compressed storage, powerful filtering, easy data access and exporting,
and integrated processing. Moreover, the system fully integrates metadata (like sensor
position) and can conjointly use point clouds with other geospatial data, such as images,
vectors, topology and other point clouds. The system also offers in-base processing
for easy prototyping, parallel processing and scales well. Lastly, the system is built
on open source technologies and generic and common hardware; therefore it can be
easily extended and customised. We test the system will several billion points from
point clouds from Lidar (aerial and terrestrial) and stereo-vision. We demonstrate 400
million pts=h loading speed, transparent-for-user and greater than 2 to 4:1 compression
ratio, filtering in the approximately 50 ms range, and output of about a million pts=s,
along with classical processing, such as object detection. 
## Download link