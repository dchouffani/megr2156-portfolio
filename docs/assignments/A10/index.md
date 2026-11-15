# A10 – Lead Screw Design

## Objective

The objective of this assignment is to design a leadscrew system by determining the minimum leadscrew diameter, rotational speed range, and maximum torque. The assignment requires selecting an appropriate bronze nut and flange, designing a crosshead that meets the strength and deflection requirements, and comparing material costs. The assignment involves parametrically modeling and assembling the components in CAD, as well as detailing the engineering lessons learned.

## Analyze

### Leadscrew - Taylor McHone

#### Minimum Diameter
<img width="167" height="467" alt="Screenshot 2026-11-15 032429" src="https://github.com/user-attachments/assets/bf84b385-2f9f-412e-9fd2-3a004e642502" />

I calculated the minimum leadscrew diameter needed to support the applied load. The total force of 2000 N was divided between two leadscrews, giving each screw a load of 1000 N. Using 1018 carbon steel with a yield strength of 64,000 psi and a safety factor of 4, I calculated the allowable stress and used the axial stress equation to determine a minimum diameter of 6.79 mm.

#### Rotational Speed
<img width="161" height="209" alt="image" src="https://github.com/user-attachments/assets/e3539a0d-62a7-43f8-b82a-8fc1f5e868d0" />

I calculated the minimum and maximum rotational speeds needed for the leadscrews to move at the required velocities of 1 mm/min and 50 mm/min. I selected a 3/8"-12 single-start leadscrew with a lead of 2.1167 mm/rev. Using the relationship between linear velocity, rotational speed, and screw lead, I calculated a minimum rotational speed of 0.4724 RPM and a maximum rotational speed of 23.62 RPM. 

#### Max Torque
<img width="304" height="410" alt="image" src="https://github.com/user-attachments/assets/83fc0858-7962-4779-a900-35e4ac82b2e8" />
<img width="216" height="212" alt="image" src="https://github.com/user-attachments/assets/00bcd8a0-be98-420c-81eb-75d728a8b152" />

I calculated the torque required to raise the applied load using the selected 3/8"-12 leadscrew. I determined the coefficient of friction and used the mean diameter, screw lead, and applied force to calculate the torque. The maximum torque was approximately 1.2314 N·m per leadscrew, giving a total torque of 2.4628 N·m for both leadscrews. These calculations assume the leadscrews and nuts are lubricated.

### Nut and Flange - Dina Chouffani
<img width="310" height="464" alt="image" src="https://github.com/user-attachments/assets/6e1e343f-d290-42f7-b960-adba80083767" />

For the nut and flange section, I analyzed the internal threads of my selected 673 bronze nut to determine whether they could support the applied load. I used a 3/8"-12 Acme thread with a 5/8-inch nut length and calculated the thread bending stress using the equation from the lecture notes. The bending stress was approximately 2,612 psi, which is below the allowable stress of 16,500 psi. The calculated safety factor was 25.3, exceeding the required safety factor of 4.
### Crosshead - Dina Chouffani
#### Strength Analysis
<img width="343" height="495" alt="Screenshot 2026-11-13 230607" src="https://github.com/user-attachments/assets/638030d0-5f08-46a8-9ede-cc061bbed587" />

I calculated the minimum required height of the crosshead based on bending stress using 6061-T6 aluminum. I used an applied load of 2000 N, a length of 300 mm, a width of 100 mm, a yield strength of 241 N/mm², and a factor of safety of 4. I used the equilibrium equations to determine the reaction forces at each support, which were both 1000 N. I then calculated the maximum bending moment and used the bending stress equation along with the allowable stress to solve for the minimum required height. The calculated height was 12.2 mm, which satisfies the bending stress requirement with a factor of safety of 4.

#### Deflection Analysis

<img width="323" height="495" alt="Screenshot 2026-11-13 232906" src="https://github.com/user-attachments/assets/37526dc2-c666-4814-911c-11e17e393b35" />

I calculated the minimum required height of the crosshead based on deflection using 6061-T6 aluminum. I used an applied load of 2000 N, a length of 300 mm, a width of 100 mm, and a maximum allowable deflection of 0.1 mm. The calculated minimum height was 26.96 mm. Since this was greater than the height required from the stress analysis, deflection controlled the design. I then substituted the calculated height back into the deflection equation and obtained a deflection of approximately 0.09999 mm, which is below the allowable 0.1 mm. Therefore, the deflection requirement was satisfied.

#### Multiview Sketch
<img width="382" height="262" alt="image" src="https://github.com/user-attachments/assets/239162d1-eb84-4510-a931-1ac0715fbd85" />

### Tabulating Costs

## Decide
_Reference your concept selection (Pugh matrix) here. How does this design follow from that decision?_

## Communicate

### Parametric Modeling

### Lessons Learned
