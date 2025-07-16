---
layout: page
title: AMI
description: 
img: assets/img/3_project/1.jpg
importance: 1
category: Work
related_publications: false
date: 2025-07-01
toc:
  sidebar: left
---

<h3>Introduction</h3>
This is one of my latest proejects. I have been tasked to make some mechanical and electronics changes to an already existing prototype to get it ready. The product is a device for automatic monitoring of insects. It takes pictures of insects and identify them using machine learning. 

<h3>Design overview</h3>
With a very limit budget i had to make a more regid design for the mounting of the electrical box (camera, PCB, Rasperry Pi ect. ) and the background plate as testing revilled it is vounable to wind. Furtermore i was tasked to integrate the modem, so the device could be accessed remotely - in this proces i also made changed to the electronic wiring and added proteccting against roddens for the cables. 

My contributions: 
- Structrual changes
- Modembox
- Cable magement & Protection

Below you will find illustraion & a small walkthrough of the areas where improvements on the design has been made. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_project/1.jpg" title="Assembled" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_project/3.jpg" title="Componets" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
</div>
<div class="caption">
    Left: Assemblled. Right: Components
</div>

<h5>Structural changes</h5>
To acount for the vibration and other factors that may be caused by the wind when the device is deployed a POM plate has been intregrated below the mounting system to provide support and make the structure more ridged. Furthermore lasercut POM plate has produced and mounted accros the two mounts connecting them and again making the device stronger. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_project/4.jpg" title="AMI structure" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
</div>
<div class="caption">
    The device when coponents is packed. Only the structual parts at the top of the case remains. 
</div>

<h5>Modem box</h5>
The modem enclosure needed to be IP-rated while maintaining compatibility with the existing construction to minimize the need for redesign. A Schneider box was selected for its size and protection class, and the modem was securely mounted using custom laser-cut plates.

Additionally, the customer requested a quick-release solution, allowing the modem to be detached and placed, for example, on a pole up to one meter away. To accommodate this, custom 3D-printed mounts were designed and integrated into both the modem box and the backboard. This allows the enclosure to remain securely fixed during operation while still being easy to remove when needed.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_project/2.jpg" title="Link A" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_project/5.jpg" title="Link B" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_project/6.jpg" title="Link B" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
</div>
<div class="caption">
    Left: A transparent view of the modem box Middel: Placement and quick fixture Right: Fixture part on modem box.
</div>


<h5>Cable magement & Protection</h5>
When the AMI is deployed in natural environments for extended periods, several factors can pose risks to the cables. Weather conditions and animals are the primary concerns. In particular, customers have previously experienced issues with rodents damaging the cables. To address this, protective sleeves were selected and implemented. These can be seen in the component image. 