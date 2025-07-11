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

<h5>Modem</h5>
