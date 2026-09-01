# A2 – Truss Stress 

## Objective

The objective of this assignment was to design a lightweight planar truss that satisfies the strength, minimum cross-sectional area, and safety factor requirements. The design process shows how and why I made each decision for my truss. SolidWorks was used to compare weight predictions with hand calculations. 

## Analyze

### Given Design Constraints

<img width="209" height="130" alt="Screenshot 2026-09-01 000716" src="https://github.com/user-attachments/assets/b249983f-2d68-4935-9c63-ac05b61ed015" />

- Applied load: P = 25 kN
- a = 0.4 m
- b = 0.3 m
- Point A: pin support
- Point B: roller support
- Truss material: ASTM A36 Steel
- Member safety factor: 3.5
- Pin material: Hardened Tool Steel
- Pin shear yield strength: 170 ksi
- Pin density: 0.278 lb/in³
- Pin safety factor: 4

### Initial Truss Geometry

<img width="422" height="314" alt="Screenshot 2026-08-31 181424" src="https://github.com/user-attachments/assets/810c4643-9a55-4d42-8cfa-2d498dfb9de6" />


I created the truss geometry using the required dimensions of a = 0.4 m and b = 0.3 m. This design has five joints and seven truss members. I used a simple geometry so that the structure could support the loads at C and D while allowing the internal forces to be determined using the method of joints without having to be complicated.

### Support Reactions

<img width="424" height="266" alt="Screenshot 2026-08-31 181652" src="https://github.com/user-attachments/assets/7fb1e5e6-43c0-4f0e-953d-12590a9653bd" />


The support reactions were determined by applying the static equilibrium equations to the entire truss. I used the sum of forces in the x-direction, the sum of forces in the y-direction, and the sum of moments to solve for the unknown reactions at the pin and roller supports. These reactions were used in solving for the internal member forces.

### Joint Free Body Diagrams and Internal Member Forces

<img width="368" height="533" alt="Screenshot 2026-08-31 181759" src="https://github.com/user-attachments/assets/bd157c7e-d162-4bbb-a16f-b4055795dfee" />

<img width="355" height="503" alt="Screenshot 2026-08-31 181900" src="https://github.com/user-attachments/assets/13c8ac76-87eb-470e-987b-e186b56aae9f" />


A free body diagram was created for each joint. The method of joints was then used with the equilibrium equations to determine the internal force in each truss element. I used the largest internal force of **20.03 kN** to determine the minimum required cross-sectional area of every truss member.

### Required Truss Member Area


<img width="351" height="325" alt="Screenshot 2026-08-31 184047" src="https://github.com/user-attachments/assets/e54ba99e-6445-499f-a0a8-58a7aaa80bb8" />


<img width="344" height="339" alt="Screenshot 2026-08-31 184157" src="https://github.com/user-attachments/assets/13119373-637a-4112-9a6f-f8efa40bae49" /> 

I used ASTM A36 steel instead of A500 structural steel, because SolidWorks did not have the A500 structural steel. I calculated the minimum required member cross-sectional area to be **280.42 mm²** using the largest internal member force, a safety factor of 3.5, and the yield strength of ASTM A36 steel. I used this area to solve for the hand calculated weight and as a minimum requirement when determining the width and depth of the truss members for the final CAD dimensions to make sure they would satisfy this minimum requirement.

### Approximate Truss Weight

<img width="350" height="353" alt="Screenshot 2026-08-31 184247" src="https://github.com/user-attachments/assets/efc8e23e-2d3d-4503-b512-c039182e208b" /> 

I calculated the truss weight so that I would have a calculated value to compare with the SolidWorks prediction. I found the total length of all seven members and multiplied this by the minimum required cross-sectional area to find the truss volume. I used the density of ASTM A36 steel and multiplied it by the truss volume to find the truss weight which was calculated to be **71.74 N**.

### Pin Free Body Diagram

<img width="322" height="119" alt="Screenshot 2026-08-31 184506" src="https://github.com/user-attachments/assets/8e145772-be69-4713-a767-0a9283e33675" />

This free body diagram shows the pin with the maximum reaction force of **8.33 kN**. I used this force and the shear stress to calculate the minimum shear area required for the pin. Single shear was used as required by the assignment.

### Required Pin Area
<img width="337" height="229" alt="Screenshot 2026-08-31 184347" src="https://github.com/user-attachments/assets/664dba93-a8d3-40d7-aa66-ef2f8b533239" />

<img width="340" height="349" alt="Screenshot 2026-08-31 184539" src="https://github.com/user-attachments/assets/ec0ab6c1-c9b0-4992-85a9-80012c015401" />

I used the 170 ksi shear yield strength of hardened tool steel and a safety factor of 4 to calculate the minimum required pin cross-sectional area as **28.44 mm²**. The area was used to find the minimum diameter since the pins are cylindrical. The minimum pin diameter calculated was approximately **6.02 mm**, which was used in the final CAD model.

### Approximate Pin Weight

<img width="346" height="449" alt="Screenshot 2026-08-31 184645" src="https://github.com/user-attachments/assets/18888102-4df0-4652-bb51-f193fa59749a" />

The pin weight was estimated using the calculated pin cross-sectional area, the selected pin length, and the specified hardened tool steel density of 0.278 lb/in³. The weight of one pin was multiplied by five to determine the combined pin weight since the truss has 5 pin joints. The calculated combined weight of the five pins was **0.129 N**.

## Decide

### Final Geometry Selection

I chose a simple truss geometry with five joints and seven members. The geometry was selected because it satisfied the required dimensions. This design allowed me to use the least amount of members and joints without overcomplicating the process of solving for the internal forces, while also keeping the weight and required area at a minimum.

### Final Member Dimensions

<img width="605" height="399" alt="Screenshot 2026-08-29 223715" src="https://github.com/user-attachments/assets/029d3c3d-9a3b-4955-a33b-b49e2e59e53c" />

<img width="529" height="280" alt="Screenshot 2026-09-01 010823" src="https://github.com/user-attachments/assets/7b24a29d-d9a1-494d-af4e-b907312ea3c2" />


A minimum member cross-sectional area of **280.42 mm²** was required for this design.

The final CAD model I designed used 30 mm wide members with a thickness of 12.04 mm to maintain the minimum cross-sectional area requirement.

At the 6.02 mm diameter pin holes, I solved for the remaining cross-sectional area:

**Anet = (30 mm - 6.02 mm)(12.04 mm)**

**Anet = 288.72 mm²**

The cross-sectional area of **288.72 mm²** is slightly greater than the required minimum area of **280.42 mm²**, which helps maintain the required cross-sectional area at the pin connections. I used a member width of **30 mm** and a thickness of **12.04 mm** because the pin holes remove area from the members at each connection. These dimensions allow the remaining cross-sectional area at the pin joints to stay above the required minimum area.

### Final Pin Design
<img width="603" height="605" alt="Screenshot 2026-09-01 002421" src="https://github.com/user-attachments/assets/8ca66cb0-269e-4427-abd8-320ad49a6b02" />


I created a custom material using the required density of 0.278 lb/in3, because SolidWorks did not have hardened tool steel. The final pins were modeled as cylinders all using the same geometry with a diameter of 6.02 mm and a length of 12.04 mm. Five pins were used, corresponding to the five truss joints. The 6.02 mm diameter was selected from the single shear strength calculation instead of being chosen randomly. A pin length of 12.04 mm was used to match the final thickness of the truss. 


## Communicate

### Final SolidWorks Model

<img width="614" height="491" alt="Screenshot 2026-08-31 174249" src="https://github.com/user-attachments/assets/6fb586dd-3105-4e28-a6f4-afa0d2618031" />

The truss minus the pins was modeled as one SolidWorks part. The pin was modeled as a single cylindrical part and was copied 5 times. The truss and pins were then imported into an assembly file to create the final assembly.

### CAD Mass Properties

<img width="347" height="590" alt="Screenshot 2026-08-31 174133" src="https://github.com/user-attachments/assets/c7f0336f-7ab1-430b-a410-0f6ad39a5ec0" />

I used SolidWorks Mass Properties to determine the mass of the completed truss using the appropriate materials. ASTM A36 steel was assigned to the truss, while the specified density of 0.278 lb/in³ was assigned to the custom hardened tool steel pins. 


The truss assembly had a predicted mass of **18.60 lb**. I converted this value to kilograms:

**m = 18.60 lb × 0.45359237 kg/lb = 8.4368 kg**

I calculated the predicted CAD weight using:

**W = mg**

**W = (8.4368 kg)(9.81 m/s²)**

**W_CAD = 82.76 N**

### Hand Calculation vs. CAD Prediction

| Method | Predicted Weight |
|---|---:|
| Hand Calculation | 71.869 N |
| SolidWorks CAD | 82.76 N |

The hand calculated total weight was approximately **71.869 N** from adding the weight of the truss and the weight of the 5 pins, while the SolidWorks model predicted a weight of **82.76 N**. The hand calculation used the minimum member cross-sectional area of 280.42 mm², so the CAD dimensions had to be selected so that the member would still maintain at least 280.42 mm² of net area after material was removed for the pin holes. Therefore, the final CAD members have a larger cross-sectional area than the minimum area assumed in the hand calculation.

### Mistakes and Design Changes

Initially, I made the thickness of the truss members **10 mm** because with a width of **30 mm**, the cross-sectional area would be **300 mm²**, which satisfied the minimum area requirement of **280.42 mm²**. After accounting for the area removed by the pin holes, the remaining area became smaller than the required minimum. I increased the thickness to **12.04 mm** so that the area at the pin connections remained above the minimum requirement while also matching the pin dimensions.

### Engineering Lessons Learned

One of the main engineering lessons I learned from this assignment is that a design does not always work out on the first try, and sometimes you have to adjust your ideas and approach as you work through the calculations. For example, I initially assumed that a member thickness of **10 mm** would be enough to satisfy the minimum area requirement. After accounting for the material removed by the pin holes, I realized that the remaining area was no longer enough, so I had to adjust my design.

I also learned the importance of working smarter, not harder. This assignment helped me realize that I need to manage my time better and know when to make changes instead of spending too much time trying to make something perfect. I learned that being efficient is just as important as being accurate and making sure the final design meets all of the requirements.

I spent approximately 10 hours symbolically and numerically solving for the internal forces and cross-sectional area, sketching and labeling free body diagrams, calculating weights, and creating the final product in SolidWorks.

### CAD File
[Download SolidWorks Truss CAD Files](Truss%20ZIP.zip)

