---
layout: post
title: Custom Load Frame
discription: Designed and built a 4-column 3D-printed load frame for testing mechanical strength in tension, compression, and bending of 3D prints
skills: 
  - Mechanical Design
  - Displacement Driven-Design
  - SOLIDWORKS CAD
  - Iterative Prototyping
  - 3D Printing
  - Arduino IDE
main-image: /IMG_8980.JPEG
---

## Overview
I designed and built a custom 4-column load frame in SOLIDWORKS to test the mechanical strength of parts and assemblies in tension, compression, and bending. The design went through several iterations, starting with a 2-column system, but limitations in the stepper motors’ force capacity led to a shift toward a 4-column design for greater load capability. The system integrates stepper motor drivers, Arduino Unos, OLED screens, load cells, amplifier boards, and SD card modules to enable real-time display, and accurate data logging for post-test analysis. By fabricating all structural components through 3D printing, I significantly reduced costs compared to industrial testing machines while maintaining functionality. My First design revolved around using a linear actuator to pull on a sample directly connected to a crane scale. This initial design had similar data logging to version two except version one used a slider pot to measure a rough displacment of th esample before ultimate faiulure occured. However, it had major drawbacks since the maximum load was around 100 lbf and there was no speed control.

---
Version 2:
{% include image-gallery.html images="IMG_8980.JPEG, IMG_8981.JPEG, LoadFrame.png" height="400" %}
---
Version 1: 
{% include image-gallery.html images="IMG_8924.JPEG, IMG_8925.JPEG, IMG_8926.JPEG, IMG_8927.JPEG" height="400" %}


---

## Accomplishments
Iterative design process improved force output and system stability.

Fully 3D-printed structure allowed rapid prototyping and cost savings.

Integrated electronics provided both live readouts and logged test data.

Capable of tension, compression, and bending experiments on custom parts.
