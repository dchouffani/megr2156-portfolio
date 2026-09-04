# A3 – Parametric and FEA

## Objective

The objective of this assignment is to create a parametric CAD model of an aluminum bar with a circular cross section, determine the length of the bar using parametric design, define parameters in SolidWorks, and compare the FEA results to the hand calculations. The FEA and hand calculations include safety factors, stress, and deflection. The parameters in SolidWorks were used to design the bar while keeping the axial deflection within the maximum of 0.009 in. The goal is to understand how FEA can be used to make sure the requirements for strength and deflection are met.

## Analyze

### Parametric Design

- Material: Aluminum
- Applied Load, F = 400 lbf
- Young's Modulus, E = 10,000,000 psi
- Maximum Axial Deflection, δ = 0.009 in
- Bar Diameter, d = 0.200 in
- Aluminum Yield Strength, Sy = 40,000 psi

**Cross-Sectional Area**

A = πd² / 4

A = π(0.200 in)² / 4

A = 0.031415926536 in²

**Parametric Length Calculation**

δ = FL / AE

where:

- δ = axial deflection
- F = applied force
- L = bar length
- A = cross-sectional area
- E = Young's Modulus

The equation was rearranged to solve for the required length:

L = δAE / F

L = [(0.009 in)(0.031415926536 in²)(10,000,000 psi)] / (400 lbf)

L = 7.0685834706 in

**Weight Calculation**

V = A × L

V = (0.031415926536 in²)(7.0685834706 in)

V = 0.22206609903 in³

W = density × V

W = (0.0975 lb/in³)(0.22206609903 in³)

W ≈ 0.02165 lb

**CAD Parameters and Equations**

<img width="601" height="255" alt="CAD equations" src="https://github.com/user-attachments/assets/1ece52c3-ed21-4d1e-9b6e-4acabc65ee90" />

<img width="563" height="344" alt="dimensions" src="https://github.com/user-attachments/assets/c8b9d71f-8123-40a1-93f7-0546a175944c" />

The diameter, applied force, Young’s Modulus, and maximum axial deflection were defined as parameters and were used to create the bar in SolidWorks. These parameters allowed the length of the bar to be automatically calculated as approximately 7.0686 in.

### Finite Element Analysis (FEA)

**Material Properties**

<img width="610" height="478" alt="Materials" src="https://github.com/user-attachments/assets/17d14003-399a-4916-bf47-938a2cdaf75d" />

A custom aluminum material was assigned with the following properties:

- Elastic Modulus = 10,000,000 psi
- Poisson's Ratio = 0.33
- Mass Density = 0.0975 lb/in³
- Yield Strength = 40,000 psi

I found the Poisson’s ratio and mass density by researching general material properties for aluminum and used the most appropriate values.

**Fixtures and Applied Load**

<img width="413" height="113" alt="forces" src="https://github.com/user-attachments/assets/ea179ea8-6806-4188-9354-f1838078fa20" />

I fixed the left side of the bar to prevent the bar from moving and applied an outward tensile force of 400 lbf on the right side. The 400 lbf force is the same force used in my parametric design so that it could later be compared to the FEA results.
 
**Mesh**

<img width="894" height="204" alt="mesh" src="https://github.com/user-attachments/assets/b1a3c90f-1a0b-4baa-afe9-4d5e710fa98d" />

I used a mesh because it divides the whole bar into smaller elements so the FEA can calculate the stress and deflection throughout the bar.

**Deflection Map**

<img width="456" height="488" alt="deflection " src="https://github.com/user-attachments/assets/e72ec1f8-fbf2-4057-a70d-5b1acea911d9" />

The deflection map shows the smallest deflection as 3.937e-32 in and the maximum deflection as 8.993e-3 in. The deflection is greatest where the 400 lbf force is applied because that is where the bar stretches the most, and smallest where the bar is fixed because it cannot move.

**von Mises Stress Map**

<img width="434" height="478" alt="Stress" src="https://github.com/user-attachments/assets/c5702c2f-1013-4a3e-b971-afd3045ffa1b" />

The von Mises stress map shows that the smallest stress is 5,635 psi and the maximum stress is 13,470 psi. The bar shows a uniform stress of approximately 12,680 psi because the cross section is uniform and there are no stress concentrations.

**Maximum Stress and Safety Factor**

σ max = 13,470 psi

Sy = 40,000 psi

13,470 < 40,000 ✓

SF = Sy/σmax

SF = 40,000/13,470

SF = 2.97

### Design Analysis

**Percent Difference**

δ given = 0.009 in

δ FEA = 0.008993 in

% Difference = |δ FEA - δ given| / δ given × 100

% Difference = |0.008993 - 0.009| / 0.009 × 100

% Difference = 0.0778%

**Pin Hole Stress Concentration, Peak Stress, and Safety Factor**

<img width="370" height="480" alt="Screenshot 2026-09-04 192515" src="https://github.com/user-attachments/assets/121ad079-9ea1-4016-86e7-446b492f2283" />

d/H = 0.20

Kt ≈ 3.15

σ nominal = 12,680 psi

σ peak = Kt(σ nominal)

σ peak = (3.15)(12,680)

σ peak = 39,942 psi

SF hole = Sy/σ peak

SF hole = 40,000/39,942

SF hole ≈ 1.00

SF hole < SF original

1.00 < 2.97

## Decide

### Design Reflection

There was no meaningful discrepancy between the given axial deflection and the one from the FEA. The percent difference was 0.0778%, The FEA deflection of 0.008993 in was less than the maximum allowable deflection of 0.009 in. Therefore, the bar meets the stiffness requirement. The results are very similar because the stress is distributed uniformly, there are no stress concentrations, and the bar has a uniform cross section. I would trust the given axial deflection more because it more accurately corresponds to the ideal geometry and loading conditions. I assumed a pin hole that was 20% of the bar's width. Using Peterson's chart, the stress concentration factor, Kt, was approximately 3.15. Using Kt, the estimated peak stress was approximately 39,942 psi, which is less than the 40,000 psi yield strength. The bar would not fail by yielding, and there would be no permanent deformation under the 400 lbf load. However, the safety factor is much lower than the original safety factor of 2.97, meaning the hole would make the bar closer to failure at the same 400 lbf load.

## Communicate

### Lessons Learned and Mistakes 
One mistake I made was rounding off the area when solving for length, which changed the true length result. I learned not to round results when using them to solve other equations. I also learned that when determining the nominal stress, I should use the stress that was throughout the whole bar rather than the maximum stress.

### Actual Time Spent

This assignment took me approximately 3 hours. Most of the time spent on this assignment was on the write up rather than designing the bar in SolidWorks.

### CAD File Download
[Download A3 SOLIDWORKS CAD File](https://github.com/dchouffani/megr2156-portfolio/raw/refs/heads/main/docs/assignments/A03/A3%20Parametric%20and%20FEA.SLDPRT)
