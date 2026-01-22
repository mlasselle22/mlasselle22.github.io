---
layout: post
title: L3 Rocket
order: 4
description: Designed and built a L3 Rocket for Certification
skills: 
  - SOLIDWORKS CAD
  - ANSYS Mechanical
  - CNC Milling
  - OpenRocket Simulation
  - DC Electronics
main-image: /IMG_8170.png
---

## Project Summary
Designed, manufactured, and flew a Level 3 Certification Rocket. The project involved 3D modeling, aerodynamic and structural simulations, CNC machining, 3D printing, and design presentations.
---

{% include image-gallery.html images="L3.JPEG, L3Matt.JPEG" height="400" %}

---

## Design
  I used OpenRocket to estimate the center of pressure and center of gravity locations for the rocket. Knowing these locations allowed me to determine the static stability of the rocket which is extremely important for a safe and predictable flight.
  
{% include image-gallery.html images="OpenRocket.png" height="300" %}

  In order for the rocket to remain stable with a good factor of safety I set up a simulation within OpenRocket to plot the static stability with respect to time with 15 mph wind gusts. The goal of the simulation was to determine a fin geometry that would allow for a roughly 1.5 caliber static stability immediately when the rocket leaves the launch pad.

{% include image-gallery.html images="Stability.png" height="300" %}

  Additionally, simulations in FinSim were performed with the fin geometry to determine what velocity divergence and flutter will happen at. The goal of running these simulations was to ensure at least a 1.5 factor of safety with respect to the flutter velocity of the fins. These simulations didn’t account for the carbon fiber layup that will be applied to the fiberglass fins. This is due to the simulations inability to do multi-material analysis. Additionally, the fins go through the walls of the airframe which makes the divergence velocity much greater than what the simulation predicts.

{% include image-gallery.html images="FinSIm2.png, FinSim1.png" height="300" %}

  I modeled the recovery bulkheads in SolidWorks, using ANSI tolerancing standards to determine appropriate clearances. Due to the larger tolerances in the commercially bought fiberglass tubes, I selected an RC8 fitment.
  Simulations in ANSYS Mechanical were made to verify that the recovery bulkheads maintained a minimum factor of safety of 2 against material yielding. The recovery bulkheads were heavily optimized to reduce weight while still maintaining the desired factor of safety. The FEA was conducted in a static case, but a dynamic analysis would have been better suited for this application.

{% include image-gallery.html images="Bulkhead.png, Bulkhead2.png" height="400" %}

---

## Manufacturing
  I manufactured the recovery bulkheads from 6061-T6 aluminum. To machine the complex geometries from weight optimization, I had to develop CAM for the part and utilize a CNC machine. I used Fusion 360 to write the CAM. Each recovery bulkhead required 7 operations that included roughing passes, drilling, filleting, and finishing passes.

{% include image-gallery.html images="Cam1.png, Cam2.png, Bulkhead3.jpg" height="350" %}

  To help stiffen the fins and prevent flutter and divergence, I used a 3K carbon fiber weave and applied three layers in a 90°–45°–90° orientation. I chose carbon fiber over fiberglass because of the greater stiffness the carbon fibers offered. Once the carbon fiber plies were fully wetted with epoxy, I used vacuum bagging to remove air bubbles which reduced internal stress concentrations and helped ensure a more complete bonding between the plies.

{% include image-gallery.html images="Layup1.jpg, Layup2.jpg" height="400" %}

---
## Flight
  The flight of the rocket wet according to plan and I achieved my level 3 certification. The rocket remained very stable throughout its flight and suffered no damage.

{% include image-gallery.html images="Ground.png, Dirt.jpg, IMG_8170.png, Close.jpg" height="400" %}

{% include youtube-video.html id="Rj_beA226i4" autoplay= "false"%} 

