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
Due to a very limited budget, I had to implement a more rigid design for mounting the electrical box as testing revealed that the original setup was vulnerable to wind. Additionally, I was tasked with integrating a modem to enable remote access to the device. During this process, I also modified the electronic wiring and added protective measures to safeguard the cables from rodent damage.

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
To account for vibrations and other factors caused by wind when the device is deployed, a POM plate was integrated beneath the mounting system to provide additional support and increase structural rigidity. Furthermore, a laser-cut POM plate was produced and mounted across the two mounting points, effectively connecting them and further strengthening the overall design.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3_project/4.jpg" title="AMI structure" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
</div>
<div class="caption">
    The device when coponents is packed. Only the structual parts at the top of the case remains. 
</div>

<h5>Modem box</h5>
The modem enclosure required an IP-rated solution while maintaining compatibility with the existing structure to minimize the need for a full redesign. A Schneider enclosure was selected for its appropriate size and protection class, and the modem was securely mounted using custom laser-cut plates.

In addition, the customer requested a quick-release mechanism that would allow the modem to be detached and repositioned—such as on a pole up to one meter away. To meet this requirement, custom 3D-printed mounts were designed and integrated into both the modem enclosure and the backboard. This solution ensures the enclosure remains securely fixed during operation while allowing for easy removal and repositioning when needed.

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
When the AMI is deployed in natural environments for extended periods, various factors can pose risks to the cabling—particularly weather conditions and animal interference. In previous deployments, customers have reported issues with rodents damaging cables. To mitigate this risk, durable protective sleeves were selected and implemented. These protective measures are visible in the component image.