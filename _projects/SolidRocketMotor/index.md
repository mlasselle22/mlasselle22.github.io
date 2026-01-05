---
layout: post
title: Solid Rocket Engine
order: 2
description: Designed, Manufactured, and Tested a Solid Rocket Engine
skills: 
  - SOLIDWORKS CAD
  - Ansys Mechanical FEA 
  - Manual Lathing
  - OpenMotor Simulation
  - 
main-image: /Cover.png
---

## Project Summary
Designed, manufactured, and test fired a solid rocket engine utilizing a custom test stand that records thrust, chamber pressure, casing temperature, and time.

---

I began the development process by defining the grain geometry and propellant characteristics using OpenMotor. This analysis was important for establishing the required motor casing dimensions as well as the anticipated chamber pressure and overall pressure rating for the system. All CAD modeling and design work was completed in SolidWorks.

For testing, I designed and built a custom test stand that incorporated a 20 kg load cell for thrust measurement, a 1600-psi pressure transducer for chamber pressure data, and a standard thermocouple for temperature monitoring.

In the initial design iterations, I experimented with a fully 3D-printed nozzle to help quantify how fast a PAHT-CF Nozzle will erode.
{% include image-gallery.html images="BeanCross.PNG, TestStandCAD.PNG, TestStand.JPEG" height="400" %}

---

The first test fire of the motor was largely unsuccessful. The fully 3D-printed nozzle experienced significant throat erosion early in the burn, which prevented chamber pressure from rising to the expected levels. As a result, the motor produced almost zero thrust and exhibited an abnormally long burn duration.
{% include youtube-video.html id="hvGe_DdZvI0" autoplay= "false"%} 
{% include image-gallery.html images="Burned.jpg" height="400" %}

---

From the data collected during the first test fire, I determined that a high-temperature resistant nozzle material such as phenolic or graphite would be required to minimize throat wear. I sourced large-diameter graphite welding rods and machined these into nozzle inserts. The throat was drilled through each insert, and I used the custom load frame I previously developed to press-fit the graphite insert into the nozzle housing using a locational fit. Finally, I machined the internal contour with a chamfer mill to create the desired convergence angle.
{% include image-gallery.html images="BeanGraphite.PNG, Graphite.jpg" height="350" %}

---

The second test fire was significantly more successful. From the flame geometry, it was apparent that the nozzle maintained a more convergent flow throughout the burn. Whereas in the first test fire the flame diameter progressively increased as the nozzle eroded.

During the second test, I successfully recorded thrust data; however, chamber pressure data was not captured. I believe this was due to selecting a pressure transducer with a measurement range that was too high for the expected operating pressure. I also believe the motor underperformed which resulted in a low chamber pressure. Based on the nozzle geometry and the use of RNX-57 propellant (which has a relatively slow burn rate), the predicted chamber pressure was approximately 60 psi. The lower than expected chamber pressure combined with the oversized sensor range likely resulted in an unusable pressure signal.

One observation from the thrust curve was that the measured thrust plateaued at roughly 0.8 lbf and did not decay toward the end of the burn. From the video of the second test fire, it can be seen that the flame decreases significantly at the end of the burn which should have showed up on the thrust curve as a decrease in thrust. I suspect the motor may have been mechanically constrained in the test stand during firing, preventing the load cell from fully capturing changes in thrust over time. As a result, the apparent flat thrust profile is likely not representative of the true motor performance.
{% include youtube-video.html id="kIxFK-ynPI4" autoplay= "false"%} }
{% include image-gallery.html images="TestFire2ThrustCurve.png" height="400" %}

---

## Closing Thoughts
Through this project, I gained significant hands-on experience ranging from data acquisition and instrumentation to pressure-vessel design and manufacturing. Moving forward, I plan to revise the sensor selection by choosing a lower-range pressure transducer. I also intend to reevaluate the test stand design to identify any mechanical constraints that may have influenced the thrust measurements. Additionally, I would like to test the motor casing using a higher-thrust propellant such as KNSU to evaluate the performance at elevated chamber pressures and thrusts.

