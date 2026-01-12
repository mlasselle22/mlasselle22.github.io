---
layout: post
title: L3 Rocket
order: 4
description: Designed and built a L3 Rocket for Certification
skills: 
  - SOLIDWORKS CAD
  - Ansys Mechanical FEA 
  - CNC Milling
  - OpenRocket Simulation
  - Project Planning
main-image: /IMG_8170.png
---

## Project Summary
Designed, manufactured, and flew a Level 3 Certification Rocket. The project involved 3D modeling, aerodynamic and structural simulations, CNC machining, 3D printing, and design presentations.
---

{% include image-gallery.html images="L3.JPEG, L3Matt.JPEG" height="400" %}

---

I began the rocket design by evaluating the achievable flight velocities for the current fin geometry, focusing on avoiding fin flutter and divergence. Simulations were performed without modeling the carbon fiber layup, providing a conservative estimate and an increased factor of safety for flutter and divergence limits.
{% include image-gallery.html images="FinSIm2.png, FinSim1.png" height="300" %}
---

Using OpenRocket simulations, I estimated the worst-case recovery load at approximately 500 lbf. I 3D modeled the bulkheads in SOLIDWORKS, designing them to effectively handle and transfer these loads throughout the airframe. I applied ANSI tolerancing standards to determine appropriate clearances and ultimately selected an RC8 fitment. I then performed FEA in Ansys Mechanical to verify that all flight components maintained a minimum factor of safety of 3 against material yielding. Additionally, the FEA allowed me to compare several aluminum alloys, enabling an optimized balance between performance and cost.
{% include image-gallery.html images="Bulkhead.png, Bulkhead2.png" height="400" %}

---

To manufacture the bulkheads, I created CAM in Fusion 360 and simulated the operations to ensure all features were machinable. I incorporated several tool changes to accommodate a wider variety of features such as fillets.
{% include image-gallery.html images="Cam1.png, Cam2.png, Bulkhead3.jpg" height="350" %}

---

I applied a carbon fiber layup to the fins to increase their stiffness and help prevent fin flutter. I selected a 3K weave and applied three layers in a 90°–45°–90° orientation. Once the carbon fiber plies were fully wetted with epoxy, I used vacuum bagging to remove air bubbles which reduces internal stress concentrations and ensure complete bonding between the plies.
{% include image-gallery.html images="Layup1.jpg, Layup2.jpg" height="400" %}

---

I flew the rocket on a M1550 motor and achieved my level 3 certification!
{% include youtube-video.html id="Rj_beA226i4" autoplay= "false"%} 

