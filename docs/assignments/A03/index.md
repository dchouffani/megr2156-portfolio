# A3 – Parametric and FEA

## Objective

The objective of this assignment is to create a parametric CAD model of an aluminum bar with a circular cross section, determine the length of the bar using defined parameters, and compare the FEA results to the calculated results. The FEA was used to find the stress and deflection of the bar, while hand calculations were used to calculate the safety factors. The goal is to understand how FEA can be used to make sure the requirements for strength and deflection are met.  

## Analyze

### Parametric Design

- Material: Aluminum
- Applied Load, F = 400 lbf
- Young's Modulus, E = 10,000,000 psi
- Maximum Axial Deflection, δ = 0.009 in
- Bar Diameter, d = 0.200 in
- Yield Strength, Sy = 40,000 psi
- Poisson's Ratio = 0.33
- Mass Density = 0.0975 lb/in³
  
**Cross-Sectional Area**

<img width="438" height="96" alt="Screenshot 2026-09-06 233849" src="https://github.com/user-attachments/assets/7e9a6b78-a709-45cf-8016-5a5647909baa" />

I calculated the cross-sectional area from the chosen diameter of 0.20 in. The area was used to find the length of the bar.

**Parametric Length**

<img width="504" height="159" alt="Screenshot 2026-09-06 232625" src="https://github.com/user-attachments/assets/e9411ece-fdde-4a70-8e16-7b155f6a2b51" />

I rearranged the direct tension elongation equation to solve for the required length. This length was later used as a parameter in SolidWorks to create the bar and perform the FEA.

**Weight**

<img width="489" height="190" alt="Screenshot 2026-09-06 232644" src="https://github.com/user-attachments/assets/93edc344-175e-4a4b-8740-5a5c3813162c" />

Using the bars volume and density of aluminum, I calculated its weight.

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

I fixed the left side of the bar to prevent the bar from moving and applied an outward tensile force of 400 lbf on the right side to cause the bar to elongate. This allowed the FEA to calculate the stress and deflection caused by the 400 lbf load.
 
**Mesh**

<img width="894" height="204" alt="mesh" src="https://github.com/user-attachments/assets/b1a3c90f-1a0b-4baa-afe9-4d5e710fa98d" />

To allow the FEA to calculate the stress and deflection throughout the bar, I used a mesh to divide it into smaller elements.

**Deflection Map**

<img width="456" height="488" alt="deflection " src="https://github.com/user-attachments/assets/e72ec1f8-fbf2-4057-a70d-5b1acea911d9" />

The deflection map shows the minimum deflection as 3.937e-32 in and the maximum deflection as 8.993e-3 in. The deflection is greatest where the 400 lbf force is applied because that is where the bar stretches the most, and smallest where the bar is fixed because it cannot move.

**von Mises Stress Map**

<img width="434" height="478" alt="Stress" src="https://github.com/user-attachments/assets/c5702c2f-1013-4a3e-b971-afd3045ffa1b" />

The von Mises stress map shows the minimum stress as 5,635 psi and the maximum stress as 13,470 psi. The bar shows a uniform stress of approximately 12,680 psi because the cross section is uniform and there are no stress concentrations.

**Maximum Stress and Safety Factor**

<img width="471" height="132" alt="Screenshot 2026-09-06 232713" src="https://github.com/user-attachments/assets/66cdd156-ec30-4d30-bb3e-c6d8a4b0f0c0" />

The maximum stress being 13,470 psi, which is less than the yield strength of 40,000 psi, means the bar is far from the point where it would start to permanently deform. The yield strength is 2.97 times greater than the maximum stress that the bar experiences.

### Design Analysis

**Percent Difference**

<img width="488" height="200" alt="Screenshot 2026-09-06 232733" src="https://github.com/user-attachments/assets/de638ea0-7baa-4e0a-b5c8-4fe763c61a06" />

I calculated the percent difference between the given axial deflection and the FEA axial deflection to see how close the FEA result was to the calculated result. The result of 0.0778% is almost negligible.

**Pin Hole Stress Concentration, Peak Stress, and Safety Factor**

<img width="370" height="480" alt="Screenshot 2026-09-04 192515" src="https://github.com/user-attachments/assets/121ad079-9ea1-4016-86e7-446b492f2283" />

<img width="492" height="222" alt="Screenshot 2026-09-06 232754" src="https://github.com/user-attachments/assets/2c2996ac-9967-47b2-9cf4-113d56820743" />

I calculated the stress concentration, peak stress, and safety factor to determine how adding a pin hole to a flat bar in tension would affect the bar under the 400 lbf load.

## Decide

### Design Reflection

There was no meaningful discrepancy between the given axial deflection and the one from the FEA. The percent difference was 0.0778%. The FEA deflection of 0.008993 in was less than the maximum allowable deflection of 0.009 in. This shows that the bar meets the stiffness requirement. The results are very similar because the FEA was based on the same design conditions I used when calculating the bar's length. I would trust the given axial deflection more because it comes from the ideal design of the bar.

I assumed a pin hole that was 20% of the bar's width, d/H=0.20. Using Peterson's chart for a hole in a flat bar in tension, the stress concentration factor, Kt, was approximately 3.15. Using Kt and the nominal stress, the estimated peak stress was 39,942 psi, which is less than the 40,000 psi yield strength. Although technically the bar would not fail by yielding and there would be no permanent deformation under the 400 lbf load, it would be very close to its limit. The safety factor is much lower than the original safety factor of 2.97, meaning the hole would make the bar considerably weaker at the same 400 lbf load. The nominal stress of the bar was 12,680 psi, while the estimated peak stress after adding the hole was 39,942 psi. Therefore, adding a substantial hole would greatly affect the safety of the bar.

## Communicate

### Lessons Learned and Mistakes 
One mistake I made was rounding off the area when solving for length, which changed the true length result. I learned not to round results when using them to solve other equations. I also learned that when determining the nominal stress, I should use the stress that was throughout the whole bar rather than the maximum stress.

### Actual Time Spent

This assignment took me approximately 3 hours. Most of the time spent on this assignment was on the write up rather than designing the bar in SolidWorks.

### CAD File Download
[Download A3 SOLIDWORKS CAD File](https://github.com/dchouffani/megr2156-portfolio/raw/refs/heads/main/docs/assignments/A03/A3%20Parametric%20and%20FEA.SLDPRT)
