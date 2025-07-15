---
layout: page
title: Custom weight
description: For education in the course MEA (Metrology, Electronics and Automation)
img: assets/img/1_project/1.jpg
importance: 1
category: Work
related_publications: false
date: 2024-11-30
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1_project/1.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The finished custom weight.
</div>

<h3>Introduction</h3>
This project was developed upon request for use in the MEA course as an educational tool in metrology. 
To this day i have build 16 of these weights & as well as a storage unit and the nessary calibration weight for the excersices. 

The system is powered by an Arduino Nano, with a custom PCB simplifying the electronic circuit.
Key components include:

- HX711 (amplifier)
- Load cell
- OLED display
- Arduino Nano

The software is accessible via LabVIEW or any IDE that supports USB communication. Additionally, the OLED display serves as a standalone visualization tool, enabling operation without a computer — only a power supply is required. 

<h3>Mechanical design</h3>
For the mechanical design, SolidWorks was used. To ensure a cost-effective production process, the design was optimized for rapid prototyping tools such as 3D printing and laser cutting.

This approach proved highly effective in a concurrent design process, where the integration of electrical components and PCB layout needed to be considered simultaneously. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1_project/5.jpg" title="CNC cut logo" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1_project/6.jpg" title="handle interface" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Issometric view. Right: Sideview.
</div>

<h3>Electrical- & PCB design </h3>
The electical design was conducted in KiCAD 8.0. The implemtation of both can be seen in the three pictures below. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1_project/2.jpg" title="CNC cut logo" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1_project/3.jpg" title="handle interface" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1_project/4.jpg" title="handle" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: PCB in kiCad. Middle: Rendering in KiCAd. Right: The implementation
</div>


<h3>Software & test</h3>
The software was developed using the Arduino platform and programmed to output a data string via the USB interface. This allows compatibility with both the Arduino IDE and LabVIEW, which the students use for data acquisition. Additionally, the measured weight is displayed on the OLED screen.

Once the software was implemented, the final step was to test the system.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    <div class="mx-auto" style="max-width: 300px;">
      {% include figure.liquid loading="eager" path="assets/img/1_project/7.jpg" title="Side View" class="img-fluid d-block mx-auto rounded z-depth-1" %}
    </div>
  </div>
</div>
<div class="caption">
    The ouput when testing with the design calibration weights. 
</div>

<h3>Storage</h3>
Since transporting 16 individual weights from the depot to the classroom can be cumbersome, a practical and efficient storage and carrying solution was required. I aimed to make the weights stackable while ensuring they remained stable during transport. The result was the following design:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1_project/8.jpg" title="CNC cut logo" class="img-fluid rounded z-depth-1" %}
    </div>
<div class="caption">
    The finished storage design.
</div>

This turned out to be one of the more challenging parts of the project, as I wanted it done properly. I used a lathe to accurately drill threaded holes in the wood to integrate the threaded rods. In the end, the effort paid off—the four finger screws can now be easily removed whenever the weights are needed.
