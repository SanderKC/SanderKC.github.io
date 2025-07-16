---
layout: page
title: Insect Sorting System
description: 
img: assets/img/2_project/1.jpg
importance: 1
category: Work
related_publications: false
date: 2024-04-30
toc:
  sidebar: left
---

<h3>Introduction</h3>
This robot is an autonomus sorting system intended for insects samples from greenland. The project was started in the summer of 2023 as a bachelor's project and the foundation for my employment at Aarhus Univerty, where i continued to develop and improve abon the design. The device is an extention to the SRS (Specimen Requsition System).

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    <div class="mx-auto" style="max-width: 400px;">
      {% include figure.liquid loading="eager" path="assets/img/2_project/1.jpg" title="Side View" class="img-fluid d-block mx-auto rounded z-depth-1" %}
    </div>
  </div>
</div>
<div class="caption">
    The finished integrated robot.
</div>

<h3>Mechanics</h3>
The ISS prototype is a fully automated sorting system featuring 30 containers, designed for seamless compatibility with the SRS. Mechanical integration is achieved through a built-in drawer, which serves both as a platform for all essential ISS components and as an ergonomic solution for lab technicians—making container replacement more efficient and user-friendly.

Key components include:

- A rotating carousel for container organization
- A pneumatically controlled linear actuator
- Extensions for the SRS flushing system
- The mechanical structure of the drawer and a hinged access door

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/2_project/2.jpg" title="Link A" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/2_project/3.jpg" title="Link B" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
</div>
<div class="caption">
    Left: SRS before. Right: SRS with the integrated ISS.
</div>


<h3>Electronics Integration</h3>
The electronics implemented in the ISS device comprise a wide range of electrical components—ranging from basic sensors and actuators to complex modules such as barcode scanners. These components work together to ensure precision, automation, and reliability across the system.

Key components include:

- Arduino Mega (Microcontroller)
- Stepper Motor & Stepper Driver
- Phototransistor
- Distance Sensor
- Barcode Scanner Module
- Microswitches (Feedback Components)
- Pneumatic Linear Actuator
- DC/DC Converter
- Additional supporting components

Each electronic part is carefully selected to fulfill a specific function within the system. The Arduino Mega serves as the central controller, orchestrating inputs and outputs, while sensors and feedback mechanisms ensure accurate system responses.

Given the diversity and number of components, integration and wire management are critical. Thoughtful PCB design and the use of a cable chain are essential to maintain order, minimize signal noise, and ensure long-term reliability.

<h3>PCB</h3>
The PCB is customed designed in KiCAD specifically as an Arduino Mega shield, serving as the central hub for all electronic components. It features clear, compact routing for stable power and signal distribution. To simplify assembly and maintenance, all connections use JST or pin headers, allowing for quick removal and replacement of individual components. The PCB is design with two planes: One ground and one Power, which is again devided in 12V, 5V & 3.3V.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/2_project/5.jpg" title="Link A" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/2_project/6.jpg" title="Link B" class="img-fluid rounded z-depth-1 custom-img" %}
    </div>
</div>
<div class="caption">
    Left: The main PCB. Right: The distance sensor PCB.
</div>


<h3>Video representation</h3>
The video below shows the prototype developed during our bachelor project. Since then, numerous improvements and upgrades have been made across the mechanical, electrical, and software components. The development process is ongoing.

{% include video.liquid path="assets/video/pexels-engin-akyurt-6069112-960x540-30fps.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}

