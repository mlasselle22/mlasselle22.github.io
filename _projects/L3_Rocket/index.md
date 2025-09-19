---
layout: post
title: L3 Rocket
description: Designed and built a L3 Rocket
skills: 
  - SOLIDWORKS CAD
  - SOLIDWORKS FEA
  - CNC Milling
  - OpenRocket Simulation
  - Project Planning
main-image: /IMG_8170.png
---

## Overview
Designed, manufactured, and flew a Level 3 Certification Rocket. The project involved 3D modeling, aerodynamic and structural simulations, CNC machining, 3D printing, and design presentations.
---

{% include image-gallery.html images="L3.JPEG, L3Matt.JPEG" height="400" %}
{% include youtube-video.html id="Rj_beA226i4" autoplay= "false"%} 
---

I began the rocket design by evaluating the achievable flight velocities for the current fin geometry, focusing on avoiding fin flutter and divergence. Simulations were performed without modeling the carbon fiber layup, providing a conservative estimate and an increased factor of safety for flutter and divergence limits.
{% include image-gallery.html images="FinSIm2.png, FinSim1.png" height="300" %}
---

Using OpenRocket simulations, I estimated the worst-case recovery load at approximately 500 lbf. I 3D modeled the bulkheads in SOLIDWORKS to distribute these loads throughout the airframe and applied ANSI tolerancing standards to determine appropriate clearances, ultimately selecting an RC8 fitment. I then performed FEA in SOLIDWORKS to ensure all flight components maintained a minimum factor of safety of 3 against material yielding. The FEA was also used to compare several aluminum alloys, allowing me to optimize for performance relative to cost.
{% include image-gallery.html images="Bulkhead.png, Bulkhead2.png" height="400" %}

---

To manufacture the bulkheads, I created CAM toolpaths in Fusion 360 and simulated them to ensure all features could be machined within tolerance. I added fillets and radii to reduce manual deburring and stress concentrations and optimized tool selection, cutting speeds, and stepovers for efficient machining and a quality surface finish.
{% include image-gallery.html images="Cam1.png, Cam2.png, Bulkhead3.png" height="400" %}

---

I applied a carbon fiber layup to the fins to increase their stiffness and help prevent fin flutter. I selected a 3K weave and applied three layers in a 90°–45°–90° orientation. Once the carbon fiber plies were fully wetted with epoxy, I used vacuum bagging to remove air bubbles which reduces internal stress concentrations and ensure complete bonding between the plies.
{% include image-gallery.html images="Layup1.jpg, Layup2.jpg" height="400" %}

---
## Accomplishments
Applied simulations to optimize fin design with the goal of preventing flutter and divergence

Balanced structural integrity and weight through careful material selection and FEA analysis.

Designed and CNC milled aluminum bulkheads.

Developed a comprehensive BOM and procurement plan to ensure timely acquisition of all components.

Delivered a technical presentation to TAPS, demonstrating design rationale, safety considerations, and expected performance.

Integrated simulation, fabrication, and project management skills to successfully bring the rocket from concept to flight-ready hardware.
