---
layout: post
title: Solid Rocket Engine
order: 1
description: Designed, Manufactured, and Tested a Solid Rocket Engine
skills: 
  - SOLIDWORKS CAD
  - Ansys Mechanical
  - Data Analysis
  - Manual Lathing
  - Additive Manufacturing
  - openMotor Simulation
    
main-image: /Cover.png
---

## Project Summary
Designed, manufactured, and test fired a solid rocket engine utilizing a custom test stand that records thrust, chamber pressure, casing temperature, and time.

---

  I utilized a free software called openMotor to establish propellent geometries. As for the propellent type, I utilized Richard Nakka’s RNX-57 and KNSB formulations. The initial impulse estimate for the RNX-57 propellent was a 59% D and with the KNSB formulation the impulse estimate was a 17% E
  
{% include image-gallery.html images="OpenMotor.png, OpenMotor2.png" height="400" %}

  The engine casing was made from aluminum 6061-T6 and turned down to size on a manual lathe. Radial bolts were used to fasten the nozzle and forward bulkhead to the casing. To prevent the aluminum casing from annealing or melting, the RNX-57 propellent was cast into a 3D printed polycarbonate liner.
The primary failure mode of the rocket engine was intentionally designed to be nozzle ejection caused by bolt tear-out in the 3D printed nozzle. This approach ensures that, in the event of an over-pressurization scenario, the nozzle releases before the motor casing bursts. Due to the anisotropic behavior of 3D printed components, I strength tested tensile samples in the orientation the nozzle will be loaded in. I used the failure stress values from the tensile testing in my tear out calculations.

{% include image-gallery.html images="Strong.png" height="400" %}

  For testing the engine, I designed and built a custom test stand that incorporated a 20 kg load cell for thrust measurement, a 1600-psi pressure transducer for chamber pressure data, and a standard thermocouple for temperature monitoring. The test stand was 3D printed out of a PA6-GF blend which made it tough and heat resistant. 

{% include image-gallery.html images="BeanCross.PNG, TestStandCAD.PNG" height="400" %}

---

## Test Fire 1
  The first test fire of the motor was largely unsuccessful. The fully 3D-printed nozzle experienced significant throat erosion early in the burn, which prevented chamber pressure from rising to the expected levels. As a result, the motor produced almost zero thrust and exhibited an abnormally long burn duration.
  
{% include youtube-video.html id="hvGe_DdZvI0" autoplay= "false"%} {% include image-gallery.html images="TestStand.JPEG, Burned.jpg" height="350" %}

  I determined that a high-temperature resistant nozzle material such as phenolic or graphite would be required to minimize throat wear. I sourced large-diameter graphite welding rods and machined these into nozzle inserts. The throat was drilled through each insert, and I press-fit the graphite insert into the nozzle housing using a tight locational fit. Finally, I machined the internal contour with a chamfer mill to create the desired convergence angle. With the tools I had available, I could only make the graphite insert converging rather than the initial design which utilized a converging-diverging nozzle.

{% include image-gallery.html images="BeanGraphite.PNG, Graphite.jpg" height="350" %}

---
## Test Fire 2
  The second test fire was significantly more successful. From the flame geometry, it was apparent that the nozzle maintained a more convergent flow throughout the burn. Whereas in the first test fire the flame diameter progressively increased as the nozzle eroded.
  
  During the second test, I successfully recorded thrust data; however, chamber pressure data was not captured. I believe this was due to selecting a pressure transducer with a measurement range that was too high for the expected operating pressure. I also believe the motor underperformed which resulted in a low chamber pressure. Based on the nozzle geometry and the use of RNX-57 propellant, the predicted chamber pressure was approximately 60 psi. The lower than expected chamber pressure combined with the oversized sensor range likely resulted in an unusable pressure signal.
  
  One observation from the thrust curve was that the measured thrust plateaued at roughly 0.8 lbf and did not decay toward the end of the burn. I suspect the motor may have been mechanically constrained in the test stand during firing, preventing the load cell from fully capturing changes in thrust over time. As a result, the apparent flat thrust profile is likely not representative of the true motor performance.

{% include youtube-video.html id="kIxFK-ynPI4" autoplay= "false"%} } {% include image-gallery.html images="TestFire2ThrustCurve.png" height="400" %}

---

## Test Fire 3

  The third test was the most successful test fire as a true thrust curve was obtained. Due to the low chamber pressures from the RNX-57 propellent, KNSB was used in the third test fire. There was a large dip in thrust at around 1.5 seconds that was due to a large inconsistence in the mixed propellent. This is likely caused by the pressure packing of the KNSB. Pressure packing was used for KNSB as there is a major fire hazard casting the propellent. However, the thrust curve obtained showed the engine produced an impulse of 9 Ns which is categorized as a 90% C engine.

{% include youtube-video.html id="Xk03UnhYxGw" autoplay= "false"%} } {% include image-gallery.html images="3Fire.png" height="400" %}

Similar to the first and second static fire, no pressure data was gathered. I suspect that the pressure transducer may be bad or have been damaged.
After three static fires, the aluminum casing is in great condition with no visible damage or discolorations. The test stand has taken no damage as well.



