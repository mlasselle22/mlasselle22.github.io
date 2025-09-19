---
layout: post
title: Custom Load Frame
order: 2
description: Designed and built a custom load frame
skills: 
  - Mechanical Design
  - Displacement Driven-Design
  - SOLIDWORKS CAD
  - Iterative Prototyping
  - 3D Printing
  - Arduino IDE
main-image: /IMG_8980.JPEG
---

## Project Summary
I designed and built a two custom load frame to test the mechanical strength of parts and assemblies.
{% include image-gallery.html images="IMG_8980.JPEG, IMG_8981.JPEG" height="400" %}
---

## Version 2: 4-Column Stepper Motor Driven Load Frame

### *Mechanical Design*
The load frame was designed in SOLIDWORKS using a 4-column architecture to provide greater load capacity and stability. The frame is capable of performing tensile, compressive, and bending tests. I chose a displacement-driven design to ensure specimens were loaded along their central axis, as any misalignment can introduce bending moments. These moments increase the principal stresses in the sample and lead to inaccurate data.

The platens were 3D-printed from carbon-fiber-reinforced polymers to maximize stiffness and minimize deflection under load. Carbon fibers within the polymer matrix significantly improve rigidity, while the platen thickness was optimized to reduce bending stresses. Since the area moment of inertia for a rectangular cross-section is given by 𝐼=1/12𝑏ℎ^3 increasing thickness (ℎ) provides a cubic improvement in stiffness against bending.

Acme threads were selected to drive the platens because their trapezoidal tooth profile is well-suited to carrying shear loads. During testing, the forces applied to the specimen are transmitted through the threaded rods primarily as shear, making Acme threads an ideal choice for strength and durability.

{% include image-gallery.html images="LoadFrame.png" height="400" %}
---

### *Hardware*
The system integrates stepper motor drivers, Arduino Unos, OLED screens, load cells, amplifier boards, and SD card modules to enable real-time display and accurate data logging for post-test analysis. All cross braces are 3D-printed and fastened to the columns using 3/8-inch bolted joints. The stepper motors are specked to produce 3 Nm of torque and are powered at 24 volts. The motors use TMC2209 drivers with a the current limiter set to 1.55A.

A 4400 lbf load cell serves as the primary force measurement device. While specimens are typically tested at 20–80% of a load cell’s maximum capacity for optimal accuracy, validation confirmed that the load reading is linear across the full range (0–4400 lbf). This ensures reliable measurements at any point on the load curve. The load cell is paired with an amplifier board running at 80 Hz for fast data collection.

An LVDT was initially considered to measure sample deformation directly between the platens. However, this introduced error because the measured displacement included both sample and system deformation, and excessive sensor noise further reduced reliability. Instead, platen separation is measured by counting stepper motor steps. This method introduces similar errors, as system deflection is included and skipped steps are not captured. However, encoders can be used in the future to ensure missed steps are accounted for.

---

### *Software*
The system is controlled using Arduino Unos, which communicate via I2C with the stepper drivers, OLED screens, load cell amplifier boards, and SD card modules. This setup enables fast communication, real-time display of a force versus time graph, and logging of data for post-test analysis.

Two push buttons on the controller allow the platens to be moved up or down at a fixed speed. In future iterations, additional testing modes will be integrated into these buttons to enable easier operation at variable speeds.
{% include image-gallery.html images="Arduino.png" height="400" %}
---

## Version 1: Linear Actuator Driven Load Frame

### *Mechanical Design*
The load frame was built around a small crane scale, a linear actuator, and a slider potentiometer sensor. The system was intended to measure mechanical strength in tension with displacement measured through the slider potentiometer. The frame utilized aluminum extrusion as the mounting bracket for all the components and all custom comonents were 3D printed. To better measure the deflection of the sample a correction function was applied to account for deflection in the crane scale hook, which attaches the sample. To determine this function, a sample that was modeled as rigid was tested, and the resulting deflection data was used to create a displacement-per-force relationship which gets subtracted form the sample data in post processing. The use of the correction function requires the assumption that the system deflection was perfectly modeled.  

{% include image-gallery.html images="IMG_8924.JPEG, IMG_8925.JPEG, IMG_8926.JPEG, IMG_8927.JPEG" height="210" %}
---

### *Hardware*
The linear actuator moves at a fixed velocity of 0.25 in/s and is not controllable. It includes a built-in voltage regulator, allowing consistent speed across an input range of 5 to 24 volts. Due to the built in voltage regulator, a lipo battery can be used to power the system as voltage sage won't affect the output speed of the actuator. All joints use M5 bolts and T nuts to allow for each part of the system to be adjusted along the aluminum extrusion.

---

### *Software*
An Arduino Uno acts as the main control board, with an SD card module used to record and log test data. The load cell amplifier board operates at 80 Hz to enable faster data collection. The slider potentiometer uses a 10-bit analog function, measuring values from 0 to 1023. A linear range within these values was determined through testing, and displacement measurements were taken within this linear range. Communication is done over I2C throughout the components while the SD card module operates on SPI. 
{% include image-gallery.html images="Code.png" height="400" %}

---

## Accomplishments
Iterative design process improved system capability and performance.   

Integrated electronics provided both live readouts and logged test data.  

Capable of tension, compression, and bending experiments on custom parts.  

