# A4 – Motor Mount

# Objective
The objective of this assignment was to design a motor mount for a brushed 24V DC gear motor with a 99.5:1 planetary gearbox that connects to a rigid wall. I was required to determine the knowns and unknowns, sketch free body diagrams, model and symbolically solve the beam stress and deflection equations, and then numerically solve for the required cross sectional geometry. I also had to include design features that minimize deflection and use parametric modeling techniques where appropriate.
    
# Analyze

## Motor Specifications and Loading

<img width="350" height="400" alt="Screenshot 2026-09-10 215347" src="https://github.com/user-attachments/assets/76baea06-9007-464f-bf8d-6170cff54134" />

<img width="1088" height="377" alt="Screenshot 2026-09-10 230332" src="https://github.com/user-attachments/assets/f156f80b-5d72-424d-b7bf-e37d48357a6d" />

## Material Properties

<img width="592" height="448" alt="material" src="https://github.com/user-attachments/assets/dc1467f8-2704-451d-8625-afbf6ec9c5ea" />

ABS was chosen from the SolidWorks material library for the motor mount. The SOLIDWORKS ABS material data did not include a yield strength, so I selected a yield strength of 30 MPa from  [SpecialChem](https://www.specialchem.com/plastics/guide/acrylonitrile-butadiene-styrene-abs-plastic) because it was consistent with the ABS material data provided in SolidWorks.


## Feature 1

<img width="316" height="140" alt="Screenshot 2026-09-11 200043" src="https://github.com/user-attachments/assets/b8ac4838-1b03-4b91-a70f-06960e850e25" />

### Free Body Diagram
<img width="326" height="77" alt="Screenshot 2026-09-11 200108" src="https://github.com/user-attachments/assets/152a273d-09d6-481c-a399-d4fa5e5f5abd" />

### Height from Stress
<img width="336" height="238" alt="Screenshot 2026-09-11 200346" src="https://github.com/user-attachments/assets/5ffbc636-ef1b-4456-bd5c-e45d7e4e42f6" />

To solve for the minimum height, I set the maximum bending stress equal to the allowable stress so the design would not exceed the allowable stress limit.

### Height from Deflection

<img width="354" height="400" alt="image" src="https://github.com/user-attachments/assets/e0dec3c9-8edd-40af-8413-1f97511be908" />

To solve for the minimum height, I set the maximum deflection equal to the allowable deflection of 0.30 mm so the design would not exceed the allowable deflection limit.

I then chose the larger height between the stress and deflection calculations because it was the minimum size that satisfied both the stress and deflection requirements.

## Feature 2

<img width="340" height="131" alt="Screenshot 2026-09-10 212324" src="https://github.com/user-attachments/assets/f1925e4f-4787-4fd0-bf6a-6ec454d8d11a" />

### Free Body Diagram

<img width="315" height="150" alt="Screenshot 2026-09-10 212455" src="https://github.com/user-attachments/assets/e1321ca2-fd6f-4101-9835-41db1d66d321" />

### Geometry

<img width="402" height="413" alt="Screenshot 2026-09-10 212410" src="https://github.com/user-attachments/assets/7b680ecf-01fe-4b47-90f6-7144d1177672" />

I solved the moment arm by subtracting the height of Feature 1 from the full length of Feature 2 since Feature 1 connects to the bottom of Feature 2. I then divided the remaining length in half to find the center of that section. I decided to place the bolt clearance holes 10 mm vertically and horizontally from the center, so I subtracted 10 mm to find the location of the lower bolt hole center. After that, I added the height of Feature 1 back so the distance was measured from the bottom of the whole bracket. I then added the bolt hole radius to reach the top edge of the lower bolt hole, which gave me the bending length. I added the 18 mm shaft length to the bending length to get the full moment arm. I included the top edge of the bolt hole in the bending length because the given free body diagram in the appendix showed the free bending region extending through the bolt hole location.

### Height from Stress

<img width="350" height="221" alt="Screenshot 2026-09-10 212546" src="https://github.com/user-attachments/assets/74839967-a024-48c3-a554-89acb81e09f9" />

To solve for the minimum height, I set the maximum bending stress equal to the allowable stress so the design would not exceed the allowable stress limit.

### Height from Deflection

<img width="332" height="284" alt="Screenshot 2026-09-10 212617" src="https://github.com/user-attachments/assets/9b749d2f-2921-4f10-8f75-ff9e6f779130" />

To solve for the minimum height, I set the maximum deflection equal to the allowable deflection of 0.30 mm so the design would not exceed the allowable deflection limit.

I then chose the larger height between the stress and deflection calculations because it was the minimum size that satisfied both the stress and deflection requirements.

## Parametric Design

<img width="590" height="425" alt="equa" src="https://github.com/user-attachments/assets/7ffa4cdd-97ea-4125-b16f-c26b82c7b5fb" />

I used global variables and equations in SolidWorks to define the dimensions of my model.

# Decide

## Dimensions

<img width="722" height="541" alt="feat 2 thick" src="https://github.com/user-attachments/assets/7074d8e4-c2af-4ee5-a94a-80edcede4995" />

For Feature 1, I chose a width and length of 40 mm because the largest diameter of the motor was 28 mm, and I wanted to ensure there was enough room around the motor. I made Feature 2 the same 40 mm width so it would align with Feature 1. I chose a length of 55 mm for Feature 2 because making it too long would increase the stress and deflection.

<img width="680" height="598" alt="Screenshot 2026-09-10 224311" src="https://github.com/user-attachments/assets/e0bd98b6-a868-4fed-a2fa-9fde26121b4e" />

The motor shaft had a diameter of 6 mm, so I made the shaft clearance hole in my design 6.5 mm. This gave the shaft enough clearance to rotate freely without touching the motor mount on feature 1.

<img width="629" height="564" alt="Screenshot 2026-09-10 230216" src="https://github.com/user-attachments/assets/a1013a3a-e28e-4bba-b6bc-1fbcda00443e" />

I used a circular sketch pattern in SolidWorks to create four 3.4 mm M3 clearance holes equally spaced around a 22 mm construction circle used to place the centers of the holes. The holes were spaced 90° apart around the center of Feature 1.

<img width="374" height="552" alt="18 2 and d" src="https://github.com/user-attachments/assets/f01858c9-acf4-400f-93d0-6520d7bec502" />

On feature 1, I made the boss clearance diameter 18.2 mm to provide enough space for the 18 mm motor boss to fully fit. I also made the recess 2 mm deep to match the depth of the motor boss.

<img width="610" height="608" alt="new feat 2 holes dim" src="https://github.com/user-attachments/assets/9a914f77-e401-4a33-a369-c85aac5320f3" />

I used a linear sketch pattern in SolidWorks to create four 3.4 mm M3 clearance holes in a square pattern on Feature 2. The four holes were arranged symmetrically around the intersection of the horizontal and vertical construction lines. Each hole center was located 10 mm horizontally and 10 mm vertically from the center, giving 20 mm of spacing between the holes in both directions.

<img width="446" height="569" alt="rib dim" src="https://github.com/user-attachments/assets/492838f0-baf5-4e0f-bc4a-ba3904089d1f" />
<img width="440" height="550" alt="rib thickness" src="https://github.com/user-attachments/assets/937f292e-a56d-4f8f-ad42-19064448a4d1" />

I added a rib extending from the top edge of Feature 2 to the base of Feature 1 to help minimize deflection. I used a rib thickness of 10 mm so it would fit between the bolt holes, and I extended the rib 4 mm onto Feature 1 so there would still be enough space for the motor.


# Communicate

## Hand Sketched Isometric View 
<img width="280" height="245" alt="Screenshot 2026-09-10 213208" src="https://github.com/user-attachments/assets/f28543f6-0fc4-40ba-9e8c-fac0c9c1de4e" />

## Final CAD Model
<img width="621" height="563" alt="final" src="https://github.com/user-attachments/assets/2e3f8759-af7b-4b50-95f3-29672e1920ea" />

## Lessons Learned

I learned how to find the cross sectional geometry using beam stress and deflection equations. One mistake I made during the design process was calculating the bending length for Feature 2. Initially, I used the height of Feature 1, but I later realized from the appendix that the bending length needed to extend to the top edge of the lower bolt hole. I reevaluated my setup and corrected my calculations.

This assignment took me approximately 6 hours to complete. Most of the time was spent determining appropriate dimensions and modeling my design in SolidWorks.

## Appendix

### Motor Mount Research

I researched different motor mounts to give me ideas for the dimensions and overall design of my motor mount.

[OUNONA L Shaped Gear Motor Mounting Bracket](https://www.walmart.com/ip/OUNONA-4pcs-Gear-Motor-Holder-Motor-L-shape-Holder-Motor-L-shape-Bracket-Motor-Mounting-Base-Mounting-Holder-Gear-Motor-Stepper-Motor-Mount-Holder/15684022296)

[NEMA 34 L Shape Motor Mounting Bracket](https://eshop.carlisgrove.com/product-p-961238.html)

## CAD File Download

[Download A4 Motor Mount SolidWorks File](https://raw.githubusercontent.com/dchouffani/megr2156-portfolio/main/docs/assignments/A04/A4%20Motor%20Mount.SLDPRT)
