---
layout: page
title: Automatic Water & fertilizer system
description: 
img: assets/img/4_project/2.jpg
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

<h3>The plan</h3>
My general plan was based on the demands for the system.The greenhouse needed to devided in to 3 section and each section needed to both be able to reseived fertilized and non-fertilized water in the same tubes. Furhtermore the freequenze and lenght of each water-circule also needs to be controlable.

I drew out a electric diagram and procided to pick out the nessary electrical components for the task:

- 1 x [Arduino_Mega](https://ardustore.dk/produkt/arduino-mega-r3-atmega2560-klon-udviklingsboard?srsltid=AfmBOooNGh_wQvUZbswxB2U4urcqqyEFGALF5rxIryue8lOSzxwg-Z_N)
- 2x [Potentiomoter](https://ardustore.dk/produkt/taper-potmeter)
- 3x [Buttom](http://ardustore.dk/produkt/push-button-pbs-110)
- 1 x [LCD-display](https://ardustore.dk/produkt/16x2-lcd-display-module-blaa)
- 1 x [Display-module](https://ardustore.dk/produkt/display-module-iic-i2c-twi-sp%e2%80%8b%e2%80%8bi-serial-interface)
- 5 x [LED](https://ardustore.dk/produkt/flashing-led-5mm)
- 3 x [Relay](https://ardustore.dk/produkt/optokobler-relae-2-kanal-5v-low-high-module)
- 6 x [Valves](https://arduinotech.dk/shop/solenoid-valve-ac-230v-1-2-straight/?gad_source=1&gad_campaignid=17511696673&gbraid=0AAAAAChom3K2wbgz2aAM3_1Pc-R-oC1uz&gclid=Cj0KCQjw-NfDBhDyARIsAD-ILeCGCwEKkrLYaP_m81hQu3e6KZqgPDZpZA3u_LxhT24rYG5CSJOJpDMaArVsEALw_wcB)'


<h3>Mechincal design</h3>
After all the selected parts was ordered i becan to design the mechanical integration. I used solidWorks to draw a control box with a userinterface. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/1.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/2.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: The interface system in SolidWorks CAD, Right: The final result after integration of electrical components. 
</div>

To give users a clear understanding of how each selected program controls the valve system, I created a custom 3D sketch of the setup. When a specific program—such as Program 1—is selected, LEDs along the water flow path illuminate, visually indicating the active sections. Each line on the right side of the sketch represents an individual greenhouse section. Additionally, the container at the bottom of the sketch illustrates the fertilizer storage; its corresponding flow path is activated under a different program, emphasizing the system’s versatility.

<h3>Electrical design</h3>
For the control interface, I selected simple buttons and knobs to adjust the frequency and duration of each watering cycle, along with an LCD display to provide real-time feedback to the user. The entire system is managed by an Arduino Mega, chosen at the time due to my familiarity with the platform and its capabilities.

Looking back, with the knowledge and experience I have gained since, I would approach certain design choices differently—these considerations are outlined in the Future Work section.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/3.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/4_project/4.jpg" title="side view" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: The electronics in the main case (12V system), Right: The box with relays. (picture is coming) 
</div>

The electrical system is built around a custom DIY Arduino shield assembled on a solderboard, mounted on a laser-cut acrylic base. While simple in construction, the setup functions reliably and effectively. The system is powered by a 12V power supply; however, since the valves operate at 230V, I made a deliberate decision to keep the 12V control system electrically isolated from the 230V power circuit to ensure safety and prevent potential interference.

<h3>Software</h3>
The software runs entirely on the Arduino Mega, utilizing its internal timing function (millis()) to manage all timing-related operations. While this approach is simple and effective for most use cases, it has a known limitation: millis() overflows after approximately 50 days of continuous operation, requiring a system reboot to reset the timer.

User input is handled via physical buttons (Up, Down, Enter), allowing navigation through the menu displayed on the LCD. Once a program is selected, the irrigation system operates based on the chosen frequency, duration, and water flow path (program). The program continues to run until either a new program is selected or the system is rebooted.

<h3>Future opdates</h3>
Since completing this project in 2023, I’ve gained significant experience in sensors, microcontrollers, and general electronics. With the knowledge I have now, I would approach several aspects of the design differently to improve performance, reliability, and usability:

- Custom PCB Design: Replacing the solderboard with a professionally designed PCB would ensure more stable signal transmission, reduce noise, and improve overall durability.

- Real-Time Clock (RTC): Integrating an RTC module would provide more accurate and reliable timekeeping, and eliminate issues related to millis() overflow.

- ESP32 Microcontroller: Upgrading to an ESP32 would offer built-in Wi-Fi capabilities, allowing remote monitoring and control of the system—an ideal feature for greenhouse automation.