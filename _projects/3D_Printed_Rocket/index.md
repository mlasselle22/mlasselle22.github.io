---
layout: post
title: 3D Printed Rocket
order: 2
description: Designed, manufactured, and launched a fully 3D-printed 6-foot-tall high-powered rocket
skills:
  - SOLIDWORKS CAD
  - Tolerancing
  - 3D Printing
  - Material Testing
main-image: /IMG_3929.JPEG
---

## Project Summary
I designed, manufactured, and flight-tested two fully 3D-printed high-powered rockets. The project included flight simulations, CAD modeling, 3D printing, material testing, and ground validation of systems.

---

## Version 2: Ultem 9085 and Nylon-10CF

### Design
For Version 2, I simulated the flight profile and stability in OpenRocket to guide my design decisions. A full CAD assembly was created in SOLIDWORKS to ensure proper component fitment with utilization of ANSI tolerances. All the parts were specifically designed to be 3D printed. The couplers were designed to withstand high bending and compressive loads.
{% include image-gallery.html images="Rocket.png, RocketCut.png" height="400" %}
---

### Manufacturing
The rocket was 3D printed on industrial grade 3D printers out of Ultem 9085 ande Nylon-10CF. Wall thicknesses and infill orientation was optimized to maximize mechanical strength.

---

### Analysis
I conducted a custom 3 point bend test on the Nylon-10Cf coupler and it successfully withstood 750 lbf without yielding. The rocket tube was tested in compression and didn't show yielding until 6000lbf. These results verified that my couplers could effectivly transfer the loads throughout the airframe of the rocket.
{% include image-gallery.html images="Bending.png, Load.png, NylonBend.jpg" height="400" %}
---

### Flight Testing
{% include image-gallery.html images="IMG_6111.jpeg" height="400" %} {% include youtube-video.html id="MT_V2mW7tbM" autoplay="false"%}


---

## Version 1: PETG and Nylon-6CF

### Design
Version 1 utilized PETG and Nylon-6CF, with the flight profile simulated in OpenRocket. A complete CAD was developed in SOLIDWORKS to allow for easy design and integration of components. All the parts were designed to be 3D printed except for the bulkheads which transfer recovery loads throughout the rocket. Version 1 utilized a 3D printed piston ejection system as the method of parachute deployment.
{% include image-gallery.html images="Piston1.png" height="400" %}
---

### Manufacturing
The rocket was printed on a custom 3D printer which was designed for printing rockets. All the printed parts had their wall and infill parameters optmized for strength while keeping the components light weight. The piston ejection system had its 3D printed parts made out of Polycarbonate and Nylon-6CF. The components were printed with a balance between nozzle diameter, layer height, and printing temperature. The parts were printed with a 0.6mm nozzle to allow for more heat transfer into the molten plastic. This was to help elongate heat conduction away from the areas being printed which in return results in a strong bond between layers. 
{% include image-gallery.html images="Printer.png" height="400" %}

---

### Material Testing
To test the strength of the PETG used in the airframe of the rocket, tensile specimens were loaded at a displacement rate of 0.25 in/s, demonstrating an ultimate strength of 3400 psi. However, due to my testing setup, the load data was not recorded at a fast enough frequency to capture the true failure stress of the material.
{% include image-gallery.html images="PETG.png" height="400" %}
---

### Flight Testing
The rocket survived the acceleration and coast phase of flight but unfortunately there was a loss of pressure during the piston actuiation and the rocket was not able to fully seperate. This led to a critical failure in the vehicle's airframe upon landing

{% include image-gallery.html images="IMG_6996.JPEG, IMG_6995.JPEG, Crash.jpg" height="400" %}
{% include youtube-video.html id="xXKfyyOq-eo" autoplay="false"%}

---

## Accomplishments
Designed, manufactured, and flight-tested two fully 3D-printed high-powered rockets.

Developed and applied material testing methods for 3D printed polymers

Validated systems through ground testing.

Integrated CAD modeling, 3D printing, material science, and experimental validation to deliver functional, high-performance rockets.

Demonstrated the ability to iterate designs between Version 1 and Version 2 to improve performance and material utilization.

