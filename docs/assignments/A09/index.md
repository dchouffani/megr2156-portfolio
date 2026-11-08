# A9 – Pulleys

## Objective

The objective of this assignment is to design a pulley system using engineering analysis to select a suitable belt, shaft, journal bearing, and supporting frame. This involves calculating belt forces, belt diameter and circumference, minimum shaft diameter under torque, and bearing pressure, linear velocity, and PV rating. The project also includes evaluating the frame design and discussing the engineering lessons learned.

## Analyze

### Belt Design

<img width="345" height="512" alt="Screenshot 2026-11-07 220257" src="https://github.com/user-attachments/assets/088a13a4-bd8d-4d53-8ef7-8639697d11d2" />

The tight side and loose side belt forces were calculated using the total belt tension and friction relationship, resulting in 8.68 lbf and 1.32 lbf, respectively. Using the normal stress equation, yield strength, and safety factor of 3, the minimum belt diameter was determined to be 0.2653 inches. The belt's outer circumference was calculated to be 19.95 inches, and a polyurethane round belt with a 5/16-inch diameter and 25-inch outer circumference was selected.
### Shaft Design

<img width="368" height="407" alt="Screenshot 2026-11-07 220327" src="https://github.com/user-attachments/assets/b416dd3d-0632-4efc-871f-b8c47f665cfa" />

The torque applied to the shaft was calculated using the pulley radius and the difference between the tight side and loose side belt forces, resulting in 11.04 lbf·in. Using the yield strength of 98,200 psi for hardened AISI 1060 steel selected from MatWeb and a safety factor of 3, the allowable shear stress was calculated to be 16,366.67 psi. The minimum shaft diameter was determined to be 0.1509 inches, resulting in a minimum cross-sectional area of 0.01789 in².

### Journal Bearing Design

<img width="335" height="461" alt="Screenshot 2026-11-07 220352" src="https://github.com/user-attachments/assets/b9668009-2a20-4ca4-8b26-c1c272877423" />
<img width="277" height="198" alt="Screenshot 2026-11-07 220939" src="https://github.com/user-attachments/assets/6191ecf1-0a48-4d64-8d0f-c79d1492a491" />

The journal bearing pressure was calculated using the radial force, minimum shaft diameter, and bearing length, resulting in 66.27 psi. The linear velocity was determined to be 59.26 ft/min, resulting in a PV rating of 3,927.05 psi·ft/min. Porous iron was selected as the journal bearing material because the calculated pressure, linear velocity, and PV rating were all below its maximum allowable limits listed in the Machinery's Handbook.

## Decide

### Engineering Analysis

<img width="350" height="310" alt="Screenshot 2026-11-07 220419" src="https://github.com/user-attachments/assets/dc8ccbcf-5c58-45e2-beca-fb3ae3a7047b" />
<img width="346" height="177" alt="Screenshot 2026-11-07 223033" src="https://github.com/user-attachments/assets/02295e5f-adfb-4cea-95d5-09bf5bd585eb" />

<img width="431" height="404" alt="ashby" src="https://github.com/user-attachments/assets/f52a9fa6-4216-4584-934f-4243c63e4204" />

An Ashby diagram comparing material strength and density was used to select 1060 aluminum alloy for the frame due to its low density and sufficient strength. The frame was designed with a length of 6.5 inches, width of 2 inches, and thickness of 0.20 inches. Using the applied force of 10 lbf and yield strength of 3,999.3 psi, the calculated safety factor was approximately 160, exceeding the required safety factor of 3 under axial loading.


## Communicate
### Lessons Learned

I learned how to use belt forces and friction to prevent slipping. I also learned how to use pressure and velocity to determine a suitable journal bearing. I learned how to use an Ashby diagram to compare different materials and choose one that best meets the needs of my pulley system.

This assignment took me approximately 3 hours to complete. 
