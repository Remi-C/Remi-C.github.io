---
layout: post
title: How street modelling has many applications
subtitle: Talking about street model for transport, autonomous vehicle, safety, public work, environment, entertainment, communication and urbanism
tags: [research]
category: research
bigimg: /img/re/sota/transport.jpeg
---
We, Mankind, are now living predominantly in cities, and mostly in big ones.
These cities are largely organized by their street network. Indeed, any activities in a city uses streets as the public interface between buildings, parks, jobs, home, leisure, and so.
Because streets concentrate so much usages, they need to be closely mapped and monitored, a tremendous challenge given the incredible amount, diversity, and rapid rate of changes.
Precisely mapping street is already pretty hard:  One has to provide the type and position of every street feature (such as sidewalks, public lighting, pedestrian crossing, etc.).
![a street map](/img/re/sota/example_street_map.jpg)
But it’s not even enough! Many applications, such as dealing with traffic, require a more complex street model containing more abstract information about how the street features are related to each other as well as city level information.
Street reconstruction is then automatically building and updating this street model using various data (street images, Lidar, GIS databases) and sophisticated algorithms.
Let’s illustrate some usages for this street map/model.


# Transport, mobility and autonomous vehicles # 
One of the primary uses of streets is to help people move. It’s fairly critical, as it will shape neighborhoods functions. Thus we need tools to understand and simulate how people move.
For pedestrian, we need a precise idea of the sidewalk geometry and of street furniture position, type, spacing along with information about where pedestrian may want to go (building entries, restaurant, subway entries, etc.). Bikes tend to go both on sidewalk and roadway, and have specific parking places (official or not!). The sidewalk height may allow or prevent some itinerary. Simulating vehicle traffic require also an idea of the street network, the traffic rules and the traffic light cycles. 
Autonomous vehicles require even more data, as we need to understand markings and traffic signs. An idea of the road width, morphology and curves may help adapt the speed and trajectories. When GPS is not reliable, precisely localizing the vehicle may require even more data, such as up-to-date street views or full textured 3D model. Furthermore, an idea of how pedestrians, bikes, and other vehicles are going to behave may avoid an accident or two.


![street model usage](/img/re/sota/transport.jpeg)

# Safety and security # 
Almost by definition, cities are a concentration of diverse people.
Any hazard may then have a big impact. A detailed geometry of the street is needed to know if a firetruck can enter the street, use its large ladder, and connect to high pressure water supply. Knowing the flammable vegetation may also come handy. Similarly, knowing if and how a stretcher can be used and the fastest path to hospital may help. But hazards are more common than that. A good idea of the paving/coating allows to anticipate accidental tripping. More generally, a very accurate modelling of the street is necessary if you want to ensure that people having trouble to see or move can navigate street objects. A very high sidewalk cannot be crossed with a stroller or wheelchair.
Streets use change radically for some big events (sports, demonstration), where crowd can form. In this case, an advanced street model may be needed to plan, manage and clean afterward. Such events can also be covered by a network of public cameras whose optimal coverage and visibility depends on a 3D model of the streets/buildings.

![street model usage](/img/re/sota/security.jpeg) 

# City management and Public work#
Although hard to believe at times, cities are actually carefully managed, which in turns requires many information about the streets.  Something seemingly as simple as garbage collection mays use frequently updated street model to detect illegal waste dumping, as well as garbage can that alter traffic flow. But in fact every street furniture has to be managed. For each public bench, markings, bollard, lights, an idea of the precise type, age and condition is required. Same goes for the condition of the paving/coating. Elevation profiles also have to be managed to ensure easy access. 
But what is above ground pales in comparison to what is underground: a host of pipes, cables, trenches and networks. Digging a hole in a street necessitate a very precise model of what is underground, lest a major inundation, gas leak or power outage be accidentally created.  Any public work also require a street model to decide what street could be blocked, and where the site huts could be positioned.

![street model usage](/img/re/sota/public_work.jpeg)

#Environment #
Streets are heavily man-made, yet inhabitants have very natural needs like … breathing. More generally, the environmental aspect is hugely important in a street. 
For instance dealing with rain water necessitate to simulate where the water is going to flow (position and capacity of drainage holes, street pavement/coating type, condition and geometry), which in turns also depends on the vegetation (tree species, size, etc.). In turn trees locally affect temperature, wind and noise propagation. Noise propagation analysis usually also requires an idea of the vehicle traffic and neighborhood usages (bars/restaurants vs houses). 
These environmental factors also affect how the inhabitants subjectively feel about a street (dark/grim vs sunny/ well-vegetated), which may change their behavior and street usage.

![street model usage](/img/re/sota/environment.jpeg)


# Entertainment, art #
We as a specie like to play! A 3D, textured model of the streets may be used for a driving game. Many pure virtual games happening in fictive simulated cities could also happen in existing cities (e.g. GTA).  But a precise street model would also be necessary for other types of game using augmented reality (game elements would be incrusted on top of the real street). Similarly, pervasive games (games where your position in the real world impacts the game) can use information from the street model for gameplay purpose. For instance, in Pokemon Go, the morphology and content of a street may influence the type of creature. 
But gaming can also be serious (serious game), as a gamified way to virtually visit a city, learn about its history, etc. 

![street model usage](/img/re/sota/game.jpeg) 

# Communication, marketing #
A very precise street model is a great tool for communication. For instance using an existing 3D textured model of a street can be modified to incorporate a future project (like a new building) and dialogue with the inhabitants.
The use of street model is also strong for geomarketing (where to locate a business for instance).  
 
# Conclusion #
Cities are growing, are becoming more complex, and with that our need to have precise, up-to-date, complex street model is growing too. Reconstructing different part of this model is a very active research field.
[Here](https://arxiv.org/abs/1803.04332) is my PhD state of the art on urban reconstruction for a much more technical overview.  

![street model usage](/img/re/sota/3d_model_usage.png)
