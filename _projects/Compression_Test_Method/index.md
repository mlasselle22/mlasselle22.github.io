---
layout: post
title: Compression Testing Method
description: Designed, built, and tested several combat robots for competitions.  
skills: 
  - Mechanical Design
  - SOLIDWORKS CAD
  - SOLIDWORKS FEA
  - CNC Milling
  - Robotics
main-image: /Comparison.png
---

## Overview
During my Summer 2025 internship, I developed and implemented an improved compression testing method for FDM 3D printed materials. The company's current method used ASTM D695-10 which defines yielding as a zero slope on the stress-strain curve, but many FDM materials do not exhibit a clear zero-slope region, leading to inconsistent data. I programmed a yield offset method in MTS TestSuite TW Elite and implemented it on a MTS Criterion Model 43, replacing the zero-slope criterion with a more reliable and accurate approach for 3D printed materials. This method improved material data accuracy and consistency, reduced technician involvement, and shortened sample preparation and 3D printing time.

---

Bad Data:
{% include image-gallery.html images="NoZeroSlope.png" height="400" %}
---
New Method:
{% include image-gallery.html images="Offset.png" height="400" %}
---
Difference in Yield Stress Values Between Methods:
{% include image-gallery.html images="Comparison.png" height="400" %}

---

## Accomplishments
Tested method on multiple FDM materials to validate repeatability.

Ensured compatibility with existing MTS TestSuite TW Elite hardware and software.

Presented findings to engineering team to demonstrate benefits and reliability improvements
