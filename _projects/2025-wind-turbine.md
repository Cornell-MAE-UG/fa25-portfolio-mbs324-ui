---
layout: project
title: Wind Turbine Design and Testing
description: Design blades for a wind turbine to optimize peak power under certain operating conditions.
technologies: [Matlab,Wind Tunnel]
image: #/assets/images/satellite-system-model.png
---

For MAE 4272 (Heat Trasnfer and Fluid Dynamics Lab), I was part of a team tasked with designing blades for a wind turbine to optimize peak power under certain operating conditions. We were responsible for selecting the airfoil, chord, length, taper, twist rate, design speed, and design RPM. For safety, the turbine had to stay below 3000 RPM and torque brake current 0.09 A. Maximum blade length was 6" and maximum chord was 2". We used a Matlab simulation to predict bending stress in our design at various conditions and found that the turbine should not operate above 7.5 m/s wind speed to preserve a factor of safety before failure. In the group, I worked on the testing procedure, pitch selection, and processing the results data.

![Airfoil Selection]({{ "/fa25-portfolio-mbs324-ui/assets/images/airfoilselect.png" | https://cornell-mae-ug.github.io/fa25-portfolio-mbs324-ui/assets/images/airfoilselect.png }}){: .inline-image-r style="width: 1000px"}

We selected an airfoil that would have a high CL/CD ratio over a wide range of AoA values to maximize useful force and therefore power. We predicted a peak power of 1.6 W at design speed 4.8 m/s (the most common wind speed in our model) and 1500 RPM. The airfoil pitch was specified as a function of optimal AoA, radial distance, and rotation rate, twisting the airfoil to maintain constant AoA for maximum CL/CD at design speed. 

![Blade CAD Showing Pitch]({{ "/fa25-portfolio-mbs324-ui/assets/images/bladecad.png" | https://cornell-mae-ug.github.io/fa25-portfolio-mbs324-ui/assets/images/bladecad.jpg }}){: .inline-image-r style="width: 1000px"}
![Wind Turbine]({{ "/fa25-portfolio-mbs324-ui/assets/images/turbinepic.png" | https://cornell-mae-ug.github.io/fa25-portfolio-mbs324-ui/assets/images/turbinepic.jpg }}){: .inline-image-r style="width: 1000px"}


We 3D-printed the blades and tested them in a wind tunnel. We controlled the wind speed and torque brake voltage. The torque on the turbine disc was increased from free spin until the rotation stopped. These power vs. RPM curves were collected for several different wind speeds in the 3-6 m/s range. Peak power of 0.9 W occured at 5 m/s, close to the design speed. However, further testing is needed to measure power at higher wind speeds between 5 and 7.5 m/s. 

![Plotting Results]({{ "/fa25-portfolio-mbs324-ui/assets/images/powercurves.png" | https://cornell-mae-ug.github.io/fa25-portfolio-mbs324-ui/assets/images/powercurves.png }}){: .inline-image-r style="width: 1000px"}
