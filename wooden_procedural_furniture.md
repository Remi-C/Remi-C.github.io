---
layout: page
title: Wooden (Computational / procedural / parametric / grammar-based) furniture
subtitle: Ideas for durable wooden furniture tailored for everybody
---

# Introduction #

People from Italy to Egypt to Japan seem to have used furniture through the millennia.
This need of furniture is not going to disappear soon, with 700 Million people visiting the largest masse furniture maker store last year.

Resources are finite, and with many billion houses, furniture need to be durable.

Wood is a good candidate for durable furniture building, as it is self-renewable. 
Yet appropriate material is not enough for durability. 
Appropriate design is also paramount (functionality as well as structure and joinery).
Thankfully, proven examples of furniture one hundred years or older exist.

In fact, highly durable furniture have been hand made for centuries. 
Although being very durable, they are not adapted for mass producing. 

# Main idea #
*Maybe computer aided design and new digital fabrication tools (laser cuter, 3D printers, etc. ) could bring 
  durable, tailored, demountable solid wood furniture to the mass?*

![Overall wooden furniture lifecycle](/img/re/furnitures/overal_wooden_furniture.jpg)
  
The digital world could help by greatly reducing the furniture fabrication time, thus making it available for the masse.
The first direction would be to use procedural modelling, mechanical simulation and assembly graph to help design, validate and customize furniture.
The second direction would be to use digital fabrication tools (CNC router, laser, waterjet, 3D printer) to help accelerate fabrication.
The key idea is this case is that digital machines would not actually fabricate the wooden furniture, but rather would fabricate templates and machining fixtures that would enormously help fabricate the furniture with usual woodworking tools.
The third direction would be to improve the documentation of the furniture so it is more easily sold, used, maintained, repaired and recycled.

# Procedural furniture modelling #
The first direction is to use procedural modelling to ease design of durable wooden furniture.
Design time is very important for high quality furniture.
A French cabinet maker common saying is that design, fabrication and finishing touches amount each to 1/3 of time.
Reducing design time is then essential.

## Procedural modelling for design ##
Time is spent for initial design, and then for each customized version of the design. 

In both cases, one solution is procedural/parametric/grammar-based modelling.
For instance the number of shelf for a library can be procedurally dependent of the height, so that changing the library height automatically add or remove shelves in the design.
The dependencies can be more complex, and can impact several parts (in the previous example, shelf fixating system would also need to be updated).

This type of capabilities has been well researched (mainly not for furniture, but for virtual building for instance) and is in fact already hinted at (at least the basics) in most modelling software (image: in solidworks).

![solidworks internet found model : https://grabcad.com/library/shelf-for-different-things-1 ](/img/re/furnitures/shelf_slid_works_combined.jpg)

Many major open questions remain, such as the most appropriate type of modelling (procedural vs grammar), the efficiency of interfaces to create the model, etc. 
Procedural modelling is also a solution to help model joins, which is a tedious and necessary task (woodworking is joining pieces of wood, with joins!).

![dovetail with sketchup https://www.popularwoodworking.com/woodworking-blogs/editors-blog/dovetails-sketchup-easier-think ](/img/re/furnitures/dovetail_sketchup.jpg)

## Mechanical analysis and guided design ##
Another important aspect for durability is the mechanical quality of the furniture.

Mechanical simulations are now very common.
Yet simulating solid wood furniture is quite difficult.
First simulating solid wood is still a challenge:
 - Properties can vary a lot even for the same wood species
 - Because wood is so anisotropic (behavior strongly depends on the fibers directions)
 - Because wood properties strongly depends on humidity content (dimensions may vary by up to 15 %!)
 
Second simulating furniture requires to simulate joins, which is hard for traditional joinery (has not been done comprehensively to the best of my knowledge)
 - It depends on the glue
 - It depends on the fitting of the join
 - It requires to quantify rigidity, a bad problem
 
Mechanical analysis could help dimension parts to optimize durability, cost, etc.
 
Besides static analysis (furniture pass/does not pass), mechanical analysis can be integrated in interactive framework,
such as in the work of Umetani et al.  (2012) : "Guided Exploration of Physically Valid Shapes for Furniture Design"
![Guided Exploration of Physically Valid Shapes for Furniture Design](/img/re/furnitures/mitra_guided_design.jpg)

The interactive capability is especially important for fluid design workflow and quick idea-to-model.
Overall, it seems that a combining and refining work is needed to obtain efficient guided design. 

## Disassembly and joinery ##
Durable furniture need to be designed to be assembled / disassembled. 
This brings several advantages:
 - Transportation is much easier, increasing re-use.
 - Furniture can more easily be a part of a modular system.
 - Broken parts can be easily isolated and rebuild.
 - Separate parts means easier fabrication (errors are less costly, handling is easier, workload can be split easier)

This topic has been researched, especially to circumvent digital fabrication tools limitations (limited printing size in 3D printer for instance).

For instance Fu et al. (2015 Computational interlocking furniture assembly) use a graph based approach to design joins so a model is interlocked.
![Computational interlocking furniture assembly](/img/re/furnitures/Computational interlocking furniture assembly.png)

From the printing community, Luo et al. (2012, Chopper: Partitioning Models into 3D-Printable Parts) split a model into printable parts, then add basic joins
![Computational interlocking furniture assembly](/img/re/furnitures/chopper.jpg)

Joins are really essential for durability. A fact that is easy to remember every time we use a creaking chair for instance.
A very beneficial side effect of having the joins designed procedurally is to generate at the same time the manufacturing process and parameters. 

# improving fabrication #
## Producing documents for fabrication ##
Fabrication relies on a large amount of documents.
This may seem wasteful, but the price of error is high in woodworking.

For starter the nomenclature and the fabrication sequences which is essential for parallelizing fabrication.
More technical documents are also needed, such as plans, cut list, etc.

All this document are direct by-products of a procedural model, and fairly easy to produce (for a concrete example, a simple sketchup plugin creates cut-list from a 3D model).

## Producing templates and machining fixtures for usual woodworking tool with digital fabrication machines ##
Woodworking tools are extremely powerful and adapted to their usages.
Trying to replace entirely these tools with digital fabrication machines (CNC router, 3D printer and laser cutter) is inefficient (a CNC router will never cut as fast as a table saw due to cutting physic).
Instead, we can use digital fabrication machines to augment classic woodworking tools by creating ad-hoc templates and machining fixtures.

![machining fixture for table router from https://www.blb-bois.com/sites/default/files/images/terme-dico-du-bois/image-multiple/2014-04/calibreur-chantournement-gabarit.jpg](/img/re/furnitures/machining_fixture_le_bouvet.jpg)

This may seem anecdotal, but in fact most of the fabricating part is spend setting tools and fabricating jigs/machining fixtures, especially when dealing with non-flat geometries.
This is especially true if taking into account the lengthy marking step when aiming for the 0.1 mm accuracy. 
Markings can also be accelerated with precision 2D printing (gluing the paper on the wood) and template laser cutting (on 4 mm medium for instance).


# improving documentation #
The third direction of improvement would be to improve the documentation.

In architecture, Building Information Model is now an important part of the architect work.
The current state of the available documentation with quality furniture is appalling.
Even the leader in masse furniture (IKEA) as a notoriously dreaded documentation.
This is mainly because producing documentation is lengthy, costly, and require computer skills.

Yet documentation is essential for maintenance, a staple of durability.

Creating a FIM: Furniture Information Model? 
In the spirit of open source, documentation can include all template/plans/model to fabricate the furniture.

# illustrating example # 

# Priorities and research proposal #

First with procedural furniture modelling, which would enable to customize a furniture based on a procedural model.
Procedural modelling is also a way to assist in joinery design.
Second with the mechanical simulation which would help validate design before prototyping, and would assist wood species selection and join dimensionning.
Third with including the way to assemble/disassemble the furniture in the design, 


The first thing is that usual digital fabrication tools (waterjet, laser cuter, 
Digital fabrication: not actually fabricate anything: fabricate templates to accelerate actual solid wood fabrication.
 from my own experience.
 

Still need a woodworker, but:
 - way easier/faster/cheaper
	* design : use parametric design to adapt to needs, rather than start from scratch each time
	* structure : software help designer cut furniture into parts, simulate design mechanical soundness, help design joins for resistance and disassembly 
	* fabricating : less tedious work required thanks to parametric templates and digital fabrication.
	* assembling: disassemble design: also means working on manageable sized parts / parts that are not too complex. (consequence of failure is not rebuild everything).
	* finishing : still place for creativity / can be customized / can be DIY + can use digital fabrication (example: laser for veneer)

What is needed for that? What exists already? (state of the art)?

 - Design : need a parametric way to represent furniture : already many possibilities ( purely procedural / grammar-based / scripts / hierarchical / module based ), including in common software (3D, solidworks, ...)
 - structure: 
  * need to split furniture into parts : many papers about this in digital fabrication for 3D printing
  * need to simulate mechanical resistance/soundness : lots of tools to do so (although no work on traditional joinery, + wood is tough to simulate)
  * need to help design joins : papers focusing on resistance or on disassembly.
 - fabricating : generating physical templates by digital fabrication is easy when the procedural model is available
 - assembling: manual can also be generated automatically (already some work on that)
 - finishing: the creative potential of veneer is enormous: tools for texturing from computer graphics community could help creativity. Easy to use laser to cut veneer.  
  
  
  


  
Furniture have been along for a long time.
Mankind revolves a lot about tools (e.g. clothes). These needs to be stored, enhanced, protected, by furniture.

From a broad perspective, furniture has seen several revolutions. 
 - Revolutions in material used with the wide spreading of metal and plastic. 
 - Revolutions in scale, with mass-producing
 - Revolution in purpose, for at least in France, the number of common furniture in a house went in one millennia from simple chest to hundreds of drawer, desk, sofa, etc. 

Like in many other fields, it seems that digital tools (computer aided design, digital fabrication) is also impacting furniture.

This leads to seriously exciting research.
Indeed, one of the issue with digital world is that it only lives inside computers.
Digital design/fabrication is a great way to materialize all these abstract stuff (software, physic, and math).

Guided design may be useful in several ways, 
Mainly to improve functionality of objects:
 - Tailored object
 - More robust objects (mechanical analysis)
 - Better assembled objects (joints / partitioning)
 - More complex objects 
 - Optimized object (for strength, weight, etc.)
 
and to help/improve the aesthetic aspect
 - help transfer style
 - help add details (pattern)
 - play with shadow/reflection/physics
 
 
## Some papers ##

Here are some papers I liked:
 - State of the Art in Methods and Representations for Fabrication-Aware Design:
  * https://www.cs.princeton.edu/~funk/star17.pdf
  * A state of the art! So useful

 - Computational Interlocking Furniture Assembly:  
  * ![locking mechanism](/img/re/furnitures/Fu et al. - 2015 - Computational interlocking furniture assembly.png)
  * Very interesting, at last no more screws.
 
 - Elasticity modulus of cabinet furniture joints: 
  * This one is interesting but lack the analysis of traditional joinery
  
 - Interactive Design and Stability Analysis of Decorative Joinery for Furniture
  * ![joinery](/img/re/furnitures/Interactive Design and Stability Analysis of Decorative Joinery for Furniture.png)
  * Work on joinery with a very computer graphics approach, nice results.
