---
layout: page
title: Wooden procedural furniture
subtitle: Ideas for durable wooden furniture tailored for everybody, using procedural methods (also called Computational ; parametric ; grammar-based depending on the research community)
---

# Purpose of this article #
This article intends to show how classic woodworking could be helped by procedural modelling, guided design, mechanical simulation and digital fabrication, the goal being to mass produce durable solid wood furniture.
Although grounded in research, this article is not an extensive state of the art.
We first start from an actual furniture building experience and outline where the digital world could have simplified/accelerated the fabrication.
Then we generalize this experience and show actual research that deals about the various parts of solid wood furniture fabrication.
Last a more practical research road map is envisioned.

![Overall Procedural solid-wood furniture](/img/re/furnitures/overal_procedural_modelling/overal_procedural_modelling.jpg) 
Illustration: starting from a furniture design idea, the designer would interactively use procedural modelling, structural analysis and procedural join modelling to explore ideas and converge to a design.
The previous tools would also be used in fabrication phase and would help harness digital fabrication tools power. 
Last helpful documents could also be generated to facilitate product fabrication, usage, repairing and recycling. 

# An example of durable, solid wood furniture design and fabrication : the modern captain bed#
[Website of the project with open sourced plan, presentation and pictures](/modern_captain_bed/).

In 2015 I decided to change my bed. I needed something very rigid (back health), practical for storage (Paris' apartments tend to be small), easily disassembled and reassembled, and of course durable (following durabilism, [a profound conviction of mine](/design_philosophy/)).

I first looked for a suitable product in few specialized company, then asked few woodworkers, without success.
Finally, I decided to design and build it myself, learning [fine wood working in the process](/2017-10-02-certified_cabinet_maker/)

Illustration: a conceptual 3D model, simplified (no joinery, no handles, simplified textures, etc.)

**click on 3D model to change view**
<div class="sketchfab-embed-wrapper"><iframe width="800" height="600" src="https://sketchfab.com/models/c7bc11224e4042eab323be94998c2b65/embed" frameborder="0" allowvr allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" onmousewheel=""></iframe>

<p style="font-size: 13px; font-weight: normal; margin: 5px; color: #4A4A4A;">
    <a href="https://sketchfab.com/models/c7bc11224e4042eab323be94998c2b65?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank" style="font-weight: bold; color: #1CAAD9;">Modern Captain Bed</a>
    by <a href="https://sketchfab.com/RCura?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank" style="font-weight: bold; color: #1CAAD9;">RCura</a>
    on <a href="https://sketchfab.com?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank" style="font-weight: bold; color: #1CAAD9;">Sketchfab</a>
</p>
</div>

## Design idea and requirements ##
I decided to get inspiration from historical captain bed (illustration below), as I estimated that marine environment constraints (sturdy, easily disassembled and reassembled, integrated storage, durable) are close to mine.
![historical captain bed](/img/re/furnitures/captain_bed/historical_nautical_captain_bed.jpg)

The main design requirements of my design are:
 - a nice wooden bed inspired by nautical captain bed,
 - a maximized amount of integrated storage (about 2m^3!, equivalent to two big closets),
 - through drawers,
 - solid wood, traditional joinery for strength and durability,
 - can come apart into small pieces (i.e. easily transportable by one person),
 - can be built with common woodworking tools.

## Design ##
### Design, drawing ###
I did most of the drawing in Sketchup, a kind of standard choice for a woodworker.
Drawing joins was so tedious that I gave up for most of them (nothing can be automate).
And when after some time thinking about the design, I decided that the bed should be less high, I ended up having to redraw everything!

![Redrawing the model](/img/re/furnitures/captain_bed/design_redraw.jpg)

**Drawing the procedural way (where the number of drawers is a parameter for instance) would have been immensely helpful.**


### Structure ###
Choosing the structure was amongst the first thing to do, as many other choices depend on it.
This step was essentially intellectual.


A bed is a kind of furniture that is under a lot of stress, as it is used 1/3 of the time.
A bed also needs to be rigid, or one person turning in the bed may disturb the other person.
Because the drawers have to go through and be accessible from either side (in case one side of the bed is against a wall),
the possibilities of structure are limited.
**Help from a guided-design software would have been much welcome**.

The bed rigidity comes from the orthogonal vertical partitions, and the frame.
![Bed main structure](/img/re/furnitures/captain_bed/structure.jpg)

### Dimensioning ###
Once having the general structure in mind, all the parts have to be dimensioned (mainly, defining the thicknesses), which tends to be difficult.
In practice, it involves looking in archives, browsing other similar designs and more notably interviewing many woodworkers to converge to something that might be OK (there is no way to know before testing it...).

Same goes for the wood species selection, a very tough problem when taking into account resistance, weight, availability, esthetics and cost!
Some parts of the structure were validated through mechanical computing (ex: how much central deformation for a slat 0,8m long, 3cm square section, when supporting 100 kg?).
Such computing was very long and painful to do, as first one has to find the mechanical properties of a given wood species (density, elasticity, etc.), then configure an available generic mechanical software. In the end, most thicknesses are 30mm for very strong parts, 24mm for strong parts, and 20mm for drawers.


**A tool to roughly simulate mechanical aspects to help validate/refine the choices would have been of great help. It would reduce the uncertainty on the final product and would avoid unnecessary over-dimensioning**.


### Joinery design ###
I decided to use traditional joinery, for durability. Moreover, the requirements to have an easily disassembled item limits gluing a lot, which in turns require mechanically stronger joins.
Some of this joins were complemented by screws and bolts, which can be worked around to go full wood, but are a very practical and reliable way to apply adjustable tension (allowing to compensate wood deformations or small conception errors).

Designing joins was an absolute pain, as dismountability has to be taken into account.
Basically, classical woodworking joins limit the degree of freedom of two pieces to 1 or 2 degree (at least a translation, sometimes a rotation).
While in theory simple, sturdiness and simplicity of the joins have to be taken into account, as well as hyper-statism (what happens when wood expands by 5% because of humidity, or something is off by 1 mm?).

To complicate things, several types of joins may have an identical locking effect, but very different durability.
This is clearly an optimization process, as shown by the mental gym one has to perform to imagine how things get together.

Illustration: The disassembly sequence of the bed, where grey arrows represent the direction of movement. Note that each movement means adequate joins.
![bed disassembly](/img/re/furnitures/captain_bed/disassembly/bed_disassembly.jpg)

**Some digital help would have been greatly beneficial, to choose the join types but also to dimension joins**, as the joins became so complicated I had to manually draw a graph of things to keep track of the work. 
![Graph of joins](/img/re/furnitures/captain_bed/graph_of_joins.jpg)

## Fabrication ##
Fabrication was different from usual professional setting, as I navigated between two associative woodshops with very different equipment, which forced me to sometimes rely on hand tools.

### List of parts, nomenclature, fabrication sequence ###
The first step of fabrication is to establish a nomenclature, a list of parts and... to buy it!
This was mostly manual, yet a single error may have a strong effect on the fabrication process.
For instance, lacking wood may add several weeks of delays has it has to be dried again in the woodshop.

Illustration: an example of nomenclature and measures to help fabrication and quality control. Because errors are so easy to make, and so costly to deal with, the more visual representations are available, the better.
![Example of nomenclature](/img/re/furnitures/captain_bed/example_nomenclature.jpg)

The fabrication sequence was mostly informal, and thus not optimized.

**Much time could have been gained by a smarter and more efficient tasks ordering and automated plan/nomenclature generation**.

### Markings and joinery ###
Markings may become very repetitive for some identical joins. I used a laser cutter to create templates for some dovetails and other joins.

I had to draw this templates manually, which is very time consuming. That is why I used this method only for a few joins (when I absolutely needed to get them identical or when a type of join had to be done multiple times).

Illustration: example of templates.
![Example of templates](/img/re/furnitures/captain_bed/templates.jpg)


**Automatically generated templates from 3D plans would have saved time and would have made the fabrication more precise.**

### Finishing touches ###
This project used only solid wood, with no veneer work, and rather simple geometry. Rather than sending, I used scrappers to prepare wood surface, then water based varnish. The finishing touches were thus rather quick.

![Example of templates](/img/re/furnitures/captain_bed/assembled_bed.jpg)

### Conclusion about the bed ###
After one year of use, I can only now assume that everything works as it should, that the bed is very solid and rigid. The storage capacity has proven to be very useful. The height were adapted to an everyday use. It is fast and easy to assemble (in about 15 minutes). It can be stored in a relatively small space (imagine if I had to store one bed and two closets instead!). It has already been moved several times with ease and without damage.
![Bed disassembled](/img/re/furnitures/captain_bed/bed_disassembled.jpg)

All in all, I spent several hundred hours to design and build the bed (well.. I still need to build the drawers).
Of course much of this time has been spent because I was still learning woodworking, and sometimes because I had to use workaround because of broken woodworking machines in the woodshop.

However, even dividing the hours spent on this bed by 4 (taking into account learning and broken tools),
it would still be too much time to fabricate it for the mass.

Since this project I took time to properly [learn](/2017-10-02-certified_cabinet_maker/) [woodworking](/woodworking_projects/) and [design](/design_projects/), to build other furniture ([a keel game](/2016-07-01-ultra_molkky/), [optimized cutting boards](/2016-12-01-cutting_board/)), to analyze a lot of existing ones, and more importantly to talk with many experienced woodworkers.
 
Besides my long time interest for digital fabrication, I also obtained a Ph.D. in computer science centered on procedural street modelling.
Because this subject had not been studied, I read many papers about procedural modelling applied to various objects, such as buildings, trees, objects.

All this made me mature and think about how to generalize my experience and bring CAD to durable woodworking. 

**The big question is then how digital fabrication and computer aided design could help to converge quickly to a better furniture design and to fabricate the furniture more efficiently.**


# Procedural modelling, mechanical simulation and digital fabrication for easier solid wood furniture fabrication #
## Introduction ##

People from Italy to Egypt to Japan seem to have used furniture through the millennia.
This need of furniture is not going to disappear soon, with 700 Million people visiting the largest mass furniture maker store last year.

Resources are finite, and with many billion houses, furniture needs to be durable.

Wood is a good candidate for durable furniture building, as it is self-renewable. 
Yet appropriate material is not enough for durability. 
Appropriate design is also essential (functionality as well as structure and joinery).
Thankfully, proven examples of furniture one hundred years or older exist.

In fact, highly durable furniture has been hand made for centuries. 
Although being very durable, they are not adapted for mass producing. 

## Main idea ##
*Maybe computer-aided design and new digital fabrication tools (laser cuter, 3D printers, etc.) could bring 
  durable, tailored, dismountable solid wood furniture to the mass?*

Illustration: general steps to create a wooden furniture, from ideas to recycling.
![Overall wooden furniture lifecycle](/img/re/furnitures/overal_wooden_furniture.jpg)
  
The digital world could help by greatly reducing the furniture fabrication time, thus making it available for the mass.
 - The first direction would be to use procedural modelling, mechanical simulation and assembly graph to help design, validate and customize furniture.
 - The second direction would be to use digital fabrication tools (CNC router, laser, waterjet, 3D printer) to help accelerate fabrication.
    The key idea is this case is that digital machines would **not** actually fabricate the wooden furniture, but rather would fabricate templates and machining fixtures that would enormously help work with usual woodworking tools.
 - The third direction would be to improve the documentation of the furniture so it is more easily sold, used, maintained, repaired and recycled.

![Overall Procedural solid-wood furniture](/img/re/furnitures/overal_procedural_modelling/overal_procedural_modelling.jpg) 
Illustration: starting from a furniture design idea, the designer would interactively use procedural modelling, structural analysis and procedural join modelling to explore ideas and converge to a design.
The previous tools would also be used in fabrication phase and would help harness digital fabrication tools power. 
Last helpful documents could also be generated to facilitate product fabrication, usage, repairing and recycling. 

## Procedural furniture modelling ##
The first direction is to use procedural modelling to ease design of durable wooden furniture.
Designing high quality furniture is really time consuming.
A French cabinet maker common precept is that design, fabrication and finishing step amount each to 1/3 of total idea-to-object time.

Reducing designing time is then essential.

### Procedural modelling for design ###
Designing time is spent for initial design, and then for each customized version of the design. 

In both cases, one solution is procedural/parametric/grammar-based modelling.

For instance the number of library's shelves can be procedurally dependent of the height, so that changing the library height automatically adds or removes shelves in the design.
The dependencies can be more complex, and can impact several parts (in the previous example the shelf fixating system would also need to be updated).

A very interesting and complex example is given in the article from Krecklau et al. (2012, Interactive Modeling by Procedural High-Level Primitives),
where they create high-level primitives to facilitate grammar usage and writing.

Illustration from the article.
![Krecklau article](/img/re/furnitures/krecklau_2012_smi_011.jpg)

This type of capabilities has been well researched (mainly not for furniture, but for virtual building for instance) and is in fact already hinted at (at least the basics) in most modelling software (illustration: an example in Solidworks).

![solidworks internet found model : https://grabcad.com/library/shelf-for-different-things-1 ](/img/re/furnitures/shelf_slid_works_combined.jpg)

Many major open questions remain, such as the most appropriate type of modelling (procedural vs grammar), the efficiency of interfaces to create the model, etc. 
Procedural modelling is also a solution to help model joins, which is a tedious and necessary task (woodworking is about joining pieces of wood, with joins!). 

Illustration: manual dovetail modelling in Sketchup.

![dovetail with sketchup https://www.popularwoodworking.com/woodworking-blogs/editors-blog/dovetails-sketchup-easier-think ](/img/re/furnitures/dovetail_sketchup.jpg)

### Mechanical analysis and guided design ###
Another important aspect for durability is the mechanical quality of the furniture.

Mechanical simulations are now very common.
Yet simulating solid wood furniture is difficult.

First, simulating solid wood is still a challenge:
 - Properties can vary a lot even for the same wood species.
 - Wood is very anisotropic (behavior strongly depends on the fibers directions).
 - Wood properties strongly depend on humidity content (dimensions may vary by up to 15 %!).
 
Second, simulating furniture requires to simulate joins,
which is hard for traditional joinery (has not been done comprehensively to the best of my knowledge).
 - It depends on the glue, wood species and the fiber direction.
 - It depends on the fitting of the join, hard to quantify for handmade joins.
 - It requires to quantify rigidity, a bad problem.
 
Mechanical analysis could help dimension parts to optimize durability, cost, etc.
 
Besides static analysis (furniture passes/does not pass), mechanical analysis can be integrated in interactive framework,
such as in the work of Umetani et al.  (2012, Guided Exploration of Physically Valid Shapes for Furniture Design)
(Illustration: from the article).

![Guided Exploration of Physically Valid Shapes for Furniture Design](/img/re/furnitures/mitra_guided_design.jpg)

The interactive capability is especially important for fluid design workflow and quick idea-to-model.
Overall, it seems that combining and refining existing work is needed to obtain efficient guided design. 

### Disassembly and joinery ###
Durable furniture needs to be designed to be assembled / disassembled. 
This brings several advantages:
 - Transportation is much easier, increasing re-use.
 - Broken parts can be easily isolated and rebuilt.
 - Furniture can more easily be a part of a modular system.
 - Separate parts means easier fabrication (errors are less costly, handling is easier, workload can be split more easily).


This topic has been researched, especially to circumvent digital fabrication tools limitations (limited printing size in 3D printer for instance).
For instance Fu et al. (2015, Computational interlocking furniture assembly) use a graph-based approach to design joins that interlock a model (some limitations: mechanical resistance not considered, joins limited to x-,y-,z-axis).
![Computational interlocking furniture assembly](/img/re/furnitures/Computational interlocking furniture assembly.png)

From the printing community, Luo et al. (2012, Chopper: Partitioning Models into 3D-Printable Parts) split a model into printable parts, then add basic joins (limitation: lacks durable joins).
![Computational interlocking furniture assembly](/img/re/furnitures/chopper.jpg)

Joins are really essential for durability. A fact that is easy to remember every time we use a creaking chair for instance.
A very beneficial side effect of having the joins designed procedurally is to generate at the same time the manufacturing process and parameters. 

## Improving fabrication ##
### Producing documents for fabrication ###
Fabrication relies on a large amount of documents.
This may seem wasteful, but the price of error is major in woodworking (both in time and materials).

The nomenclature and the fabrication sequences could be generated automatically, this is essential for parallelizing fabrication.
More technical documents are also needed, such as plans, cut list, etc.

All this document are direct by-products of a procedural model, and fairly easy to produce (for a concrete example, a simple Sketchup plugin creates cut-list from a 3D model).

### Producing templates and machining fixtures for usual woodworking tool with digital fabrication machines ###
Woodworking tools are extremely powerful (several kW each usually) and adapted to their usages.
Trying to replace entirely these tools with digital fabrication machines (CNC router, 3D printer and laser cutter) is inefficient (a CNC router will never cut as fast as a table saw due to cutting physic for instance).
Instead, we can use digital fabrication machines to augment classic woodworking tools by creating ad-hoc templates and machining fixtures.
(Illustration: example of a classic machining fixture, credits: Le Bouvet magazine)

![machining fixture for table router from https://www.blb-bois.com/sites/default/files/images/terme-dico-du-bois/image-multiple/2014-04/calibreur-chantournement-gabarit.jpg](/img/re/furnitures/machining_fixture_le_bouvet.jpg)

This may seem anecdotal, but in fact most of the fabricating part is spent setting tools and fabricating jigs/machining fixtures, especially when dealing with non-flat geometries.
This is especially true if taking into account the lengthy marking step when aiming for the 0.1 mm accuracy. 
Markings can also be accelerated with precision 2D printing (gluing the paper on the wood) and template laser cutting (on 4 mm medium for instance, which is then used to report the marks).

## Improving documentation ##
The third direction of improvement would be to improve the documentation.
Documentation is essential for maintenance, repair and recycling, a staple of durability.

Yet the current state of the available documentation with quality furniture is appalling.
Even the leader in mass furniture has a notoriously dreaded documentation.
This is mainly because producing documentation is lengthy, costly, and requires computer skills.

In architecture, Building Information Model (BIM) is now an important part of the architect work.
BIMs contain a lot of information, not always useful for furniture, but maybe we could focus on the core and create FIM: Furniture Information Model? 
In the spirit of open source, documentation can include all template/plans/model to fabricate the furniture, as well as mechanical characteristics and material provenance and recycling options.


# Priorities and research roadmap example #
This article introduces a lots of research avenues, potentially much more than what can be done by one person.

The described procedural woodworking ideas can be prioritized so they are tested and published incrementally while minimizing risks.

For instance, I would try to follow this broad steps (depending on available collaboration of course): 
 - (about 6 months): state of the art article, contact with specialized labs/individuals on the subject. Full article.
 -  create an interactive procedural modelling of furniture and joins: softwar (design choices are not assisted), then build few pieces of furniture with the outputted plans (timed). Short article/poster.
 - automate generation of fabrication sequences, templates and machining fixtures from the procedural model. Re-build same pieces of furniture (timed), compare times. Full article.
 - guided joins selection based on the interlocking paper, with friction, complexity and very basic resistance taken into account. Full article.
 - in *parallel* (depending on the collaborations)
  * propose a Furniture Information Model
  * work on a basic mechanical analysis adapted to traditional joinery
  * work on guided design based on mechanical analysis
  * computer graphics texturing method applied to veneer
 - long term research : mixed materials (reclaimed wood/metal, leather, veneer), 3D sculpting / style grammar

