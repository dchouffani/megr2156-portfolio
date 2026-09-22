# A5 – Bracket Design

## Objective

The objective of this assignment is to design a bracket to hold a horizontal force applied symmetrically by a strap. I will conduct stress analysis to determine appropriate dimensions for each structural feature and generate free body diagrams (FBDs) to visualize the forces and constraints. I will state known and unknown variables, assumptions, and algebraic models for the stress calculations. As well as, perform stiffness analysis to determine the minimum required dimensions based on the deflection constraints. The stress and stiffness results will be compared to determine the required dimensions and I will create detailed multiview sketches using the dimensions from both analyses.

## Analyze

<img width="367" height="168" alt="Screenshot 2026-09-21 223043" src="https://github.com/user-attachments/assets/92e28b1a-bdc2-485b-a4e8-0b7514b9ee9c" />

<img width="273" height="195" alt="Screenshot 2026-09-21 223110" src="https://github.com/user-attachments/assets/fd26ff4c-18d6-4138-b6fa-3b91a372d925" />

<img width="604" height="477" alt="Screenshot 2026-09-21 223723" src="https://github.com/user-attachments/assets/607cba63-ac59-468f-bff8-2f0a7196d577" />

I selected ASTM A36 steel as the material for my bracket. I used a safety factor of 4, a maximum allowable deflection of 0.005 in, and an applied load of 600 lbf. I used these values for the stress and stiffness analyses to find the dimensions for each feature.

<img width="358" height="455" alt="Screenshot 2026-09-21 210114" src="https://github.com/user-attachments/assets/16b1aede-5d3f-4447-81b3-141d66ba1f3b" />

<img width="365" height="530" alt="Screenshot 2026-09-21 225742" src="https://github.com/user-attachments/assets/9aafec7a-fc38-4860-a4d0-6fbce34afea8" />

<img width="359" height="486" alt="Screenshot 2026-09-21 210223" src="https://github.com/user-attachments/assets/158bbc97-3e38-46fd-a5c6-c0e1baedfe1f" />

<img width="368" height="555" alt="Screenshot 2026-09-21 210241" src="https://github.com/user-attachments/assets/ecbdc65e-e6a0-472d-8349-259cb62eb0f8" />

<img width="380" height="547" alt="Screenshot 2026-09-21 210301" src="https://github.com/user-attachments/assets/5c06c138-c579-4461-bc8f-53e53cf6a001" />

<img width="366" height="582" alt="Screenshot 2026-09-21 210320" src="https://github.com/user-attachments/assets/27850880-1424-4bee-a08c-2f296da5e881" />

<img width="362" height="478" alt="Screenshot 2026-09-21 210334" src="https://github.com/user-attachments/assets/3f0a071c-8537-45ba-92c3-f0bca95660eb" />

<img width="352" height="564" alt="Screenshot 2026-09-21 210352" src="https://github.com/user-attachments/assets/b21e8868-3c04-4ce9-9682-17a1d8143d36" />

<img width="367" height="497" alt="Screenshot 2026-09-21 210409" src="https://github.com/user-attachments/assets/000bf51b-aadb-41f0-b126-8f205a84a84b" />

<img width="370" height="565" alt="Screenshot 2026-09-21 210427" src="https://github.com/user-attachments/assets/68501709-9210-4994-99af-d14c5c8f6115" />

<img width="399" height="565" alt="Screenshot 2026-09-21 210443" src="https://github.com/user-attachments/assets/2ea8f696-0b24-4465-9777-931872dabb14" />


## Decide

### Design Assumptions

**Feature A:**  
I selected a length of 1 in because the strap has a thickness of 0.75 in. The additional length allows clearance for the strap.

**Feature B:**  
I selected the width of Feature B to equal the diameter of Feature A so the two features align. I selected a length of 1 in to allow enough space for Feature A.

**Feature C:**  
I assumed a length of 2.5 in because the given dimensions result in **a + 2b ≈ 2.49 in**, so 2.5 in provides a practical dimension that closely matches the required geometry. I selected a width of 1 in to match the length of Feature A.

**Feature D:**  
I selected a width of 1 in to maintain consistency with the other part dimensions. I selected a height of 1.5 in to match the given dimension **c**.

**Feature E:**  
I selected a width of 1 in to maintain consistency with the rest of the part. I selected a length of 0.9990 in based on the given **b** dimension so that Feature E fits within the required geometry without interfering with the surrounding features.

## Communicate

**Lessons Learned:**

I learned how to determine dimensions using stress and deflection analyses and how to determine which value governs the design when selecting the final dimensions.

**Governing Failure Mode:**  
For Feature A, the calculated diameter of 0.8709 in from the stress analysis governed over the calculated diameter of 0.381 in from the stiffness analysis. The stress diameter meets both the stress and stiffness requirements.

**Error Propagation:**  
I carried the diameter of Feature A into Feature B and used it as the width of Feature B. There was no error in my calculation, but I made sure I calculated the correct diameter before using it in Feature B.

**Assumption Sensitivity:**  
For Feature E, I assumed a cantilever beam with a point load at its free end because the bracket restricted movement on one end while allowing movement on the other end. If this assumption were different, the dimensions of Feature E would change because the bending and deflection equations would be different.

This assignment took me approximately 5 hours to determine the assumptions I wanted to use and to calculate the required dimensions using stress and stiffness analyses.
