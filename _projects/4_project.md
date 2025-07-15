---
layout: page
title: Automatic Water & fertilizer system
description: 
img: assets/img/4_project/1.jpg
importance: 1
category: Fun
related_publications: false
date: 2023-01-09
toc:
  sidebar: left
---

<h3>Introduktion</h3>
My father is a micro-farmer with a lifelong passion for growing more — and more uniquely — than the average person. For as long as I can remember, he has cultivated everything from carrots and potatoes to rare and specialty crops such as blue potatoes, black carrots, and specially ordered flowers, all grown for local restaurants and not typically found in supermarkets.

A few years ago, he received a shipment of flowers that mistakenly included a giant pumpkin seed. That seed sparked a new interest — and eventually a hobby — that drew me in as well. As it turns out, growing a giant pumpkin is practically a science in itself.

I’ve worked alongside my father in the field since I was very young. So, when he asked if I could design a system to automate the watering and fertilization process for his new passion, I was more than happy to take on the challenge.

If you're interested, you can take a look at the [greenhouse](/projects/5_project/) structure I also designed. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/1.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The interface system & the control valve. 
</div>

<h3>The plan</h3>
My general plan was based on the demands for the system.The greenhouse needed to devided in to 3 section and each section needed to both be able to reseived fertilized and non-fertilized water in the same tubes. Furhtermore the freequenze and lenght of each water-circule also needs to be controlable.

I drew out a diagram and procided to pick out the nessary electrical components for the task:

- [Arduino_Mega](https://ardustore.dk/produkt/arduino-mega-r3-atmega2560-klon-udviklingsboard?srsltid=AfmBOooNGh_wQvUZbswxB2U4urcqqyEFGALF5rxIryue8lOSzxwg-Z_N)
- 2x [Potentiomoter](https://ardustore.dk/produkt/taper-potmeter)
- 3x [Buttom](http://ardustore.dk/produkt/push-button-pbs-110)
- 1 x [LCD-display](https://ardustore.dk/produkt/16x2-lcd-display-module-blaa)
- 1 x [Display-module](https://ardustore.dk/produkt/display-module-iic-i2c-twi-sp%e2%80%8b%e2%80%8bi-serial-interface)
- 5 x [LED](https://ardustore.dk/produkt/flashing-led-5mm)
- 3 x [Relay](https://ardustore.dk/produkt/optokobler-relae-2-kanal-5v-low-high-module)
- 6 x [Valves](https://arduinotech.dk/shop/solenoid-valve-ac-230v-1-2-straight/?gad_source=1&gad_campaignid=17511696673&gbraid=0AAAAAChom3K2wbgz2aAM3_1Pc-R-oC1uz&gclid=Cj0KCQjw-NfDBhDyARIsAD-ILeCGCwEKkrLYaP_m81hQu3e6KZqgPDZpZA3u_LxhT24rYG5CSJOJpDMaArVsEALw_wcB)'


- [Screen](https://funnyplaying.com/products/3-0-inch-ips-agb-laminated-kit)
- [LED](https://ardustore.dk/produkt/flashing-led-5mm)
- [USB-C / battery mod](https://funnyplaying.com/products/gba-li-ion-rechargeable-battery-typec-module)
- [button](https://funnyplaying.com/products/agb-custom-buttons)
- [Silicone pads](https://funnyplaying.com/products/replacement-silicone-pads-for-gameboy-advance)

<h3>The work</h3>
Due to the selected parts, the amount of work to put the modded GameBoy together was minimal. It only took a short Friday afternoon after work. The most complicated part was the soldering needed for the new display overlay controls, which consisted of three wires that allowed the overlay to be controlled with the GBA buttons instead of the touch sensor built into the screen.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/soldering1.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The wires soldered to the new display PCB.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/soldering2.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The wires soldered to the GBA PCB.
</div>

After that, it was mostly a matter of putting the parts in the right spots and screwing everything together.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/Internals.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The assembled internals 
</div>

<h3>The results<\h3>

Once the back shell was screwed down, I was left with a fully modded GameBoy Advance.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/new.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The finished product show the pokemon sapphire start screen.  
</div>

And it glows!

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/GID.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The finished product show the pokemon sapphire start screen.  
</div>

