---
layout: post
title: Compression Testing Method for Stratasys
order: 3
description: Refined Stratasys Compression Testing Method to Improve Accuracy and Reliability in Material Data
skills: 
  - Test Method Development
  - Material Testing
  - Data Collection and Analysis
  - 3D Printing
  - Excel Automation
  - MTS TestSuite TW Elite
main-image: /Comparison.png
---

## Overview
During my Summer 2025 internship for Stratasys, I developed and implemented an improved compression testing method for FDM 3D printed materials. The company's current method used ASTM D695-10 which defines yielding as a zero slope on the stress-strain curve, but many 3D printed materials do not exhibit a clear zero-slope region, leading to inconsistent data. I programmed a yield offset method in MTS TestSuite TW Elite and implemented it on a MTS Criterion Model 43, replacing the zero-slope criterion with a more reliable and accurate approach for 3D printed materials. This method improved material data accuracy and consistency, reduced technician involvement, and shortened sample preparation and 3D printing time. 

---
## **Old Method**
Since the graph never exhibits a true zero-slope, the yield data is often taken at the end of the stress–strain or force–displacement curve. This approach introduces several inaccuracies, the most significant being yield stresses that do not reflect the point at which the material actually yields. Consequently, the corresponding strain at yielding is also misrepresented. Unfortunately, this flawed data has been reported to customers for years.
{% include image-gallery.html images="NoZeroSlope.png" height="400" %}
To determine whether the ASTM D695-10 standard is applicable to 3D-printed polymers, I tested an injection-molded sample to see if it exhibited the zero-slope region specified by the standard. The results clearly showed that 3D-printed polymers do not exhibit the same yielding behavior as injection-molded polymers.
{% include image-gallery.html images="Data.png" height="400" %}
---
## **New Method**
The method I developed utilizes an offset yield criteria as a measure of material yielding. An offset is taken from the linear region on a stress strain curve and offset but either 0.2%, 0.5%, or 1% depending on the data that is requested. These offset yield criteria values accuretely represent that materail yielding. All the programming for this new method was done in *MTS TestSuite TW Elite* 
{% include image-gallery.html images="Offset.png" height="400" %}
---
## **Difference in Yield Stress Values Between Methods**
There was a substantial difference in the yield stress values obtained using the previous test method compared to those measured with the new method I developed. The previous approach consistently overestimated yield stress values, whereas the method I implemented produced results that more accurately reflect the true yield stress of the bulk polymer material. The standard deviations in the data also show a significant improvement. With the old method, yield stress standard deviations could be as high as ±5,000 psi, an unreasonably large variation. In contrast, the new method produces standard deviations in the range of ±200 psi. This improvement not only provides a more precise representation of material behavior but also greatly enhances the reliability and consistency of the measurements. 
{% include image-gallery.html images="Comparison.png" height="400" %}

---

## Accomplishments
Developed and implemented an improved compression testing method for FDM 3D-printed materials

Programmed the offset yield method in MTS TestSuite TW Elite for the MTS Criterion Model 43, enabling automated, accurate yield stress measurements.

Validated that traditional ASTM D695-10 testing is not appropriate for 3D-printed polymers by comparing results to injection-molded samples.

Achieved a substantial increase in data accuracy.

Gained hands-on experience with material characterization, experimental design, and automation of testing software for polymer evaluation.
