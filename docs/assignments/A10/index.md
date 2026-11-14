# A10 – Lead Screw Design

## Objective

The objective of this assignment is to design a leadscrew system by determining the minimum leadscrew diameter, rotational speed range, and maximum torque. The assignment requires selecting an appropriate bronze nut and flange, designing a crosshead that meets the strength and deflection requirements, and comparing material costs. The assignment involves parametrically modeling and assembling the components in CAD, as well as detailing the engineering lessons learned.

## Analyze

### Leadscrew Diameter

### Nut and Flange

### Crosshead
#### Strength Analysis
<img width="343" height="495" alt="Screenshot 2026-11-13 230607" src="https://github.com/user-attachments/assets/638030d0-5f08-46a8-9ede-cc061bbed587" />

I calculated the minimum required height of the crosshead based on bending stress using 6061-T6 aluminum. I used an applied load of 2000 N, a length of 300 mm, a width of 100 mm, a yield strength of 241 N/mm², and a factor of safety of 4. I first drew a free-body diagram and used the equilibrium equations to determine the reaction forces at each support, which were both 1000 N. I then calculated the maximum bending moment and used the bending stress equation along with the allowable stress to solve for the minimum required height. The calculated height was 12.2 mm, which satisfies the bending stress requirement with a factor of safety of 4.

#### Deflection Analysis

<img width="347" height="529" alt="Screenshot 2026-11-13 230630" src="https://github.com/user-attachments/assets/bf82a6eb-327d-4d46-91d6-a37be3e6413a" />

I calculated the minimum required height of the crosshead based on deflection using 6061-T6 aluminum. I used an applied load of 2000 N, a length of 300 mm, a width of 100 mm, and a maximum allowable deflection of 0.1 mm. I substituted the moment of inertia equation into the deflection equation and rearranged it to solve for the height. The calculated minimum height was 26.96 mm. Since this was greater than the height required from the stress analysis, deflection controlled the design. I then substituted the calculated height back into the deflection equation and obtained a deflection of approximately 0.09999 mm, which is below the allowable 0.1 mm. Therefore, the deflection requirement was satisfied.

#### Multiview Sketch

### Tabulating Costs

## Decide
_Reference your concept selection (Pugh matrix) here. How does this design follow from that decision?_

## Communicate

### Parametric Modeling

### Lessons Learned
