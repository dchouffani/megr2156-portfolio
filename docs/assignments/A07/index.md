# A7 –  FEA on Bracket

## Objective
The objective of this assignment is to use Finite Element Analysis (FEA) to improve the bracket design from previous assignments. The goal is to ensure high stiffness, strength, and lightweight optimization through iterative design. Multiple FEA simulations will be conducted, refining the geometry based on the results. Static stress analysis will be performed, including constraints, loading, and meshing selection. and the data will be interpreted by identifying maximum stress, displacement, and safety factors. The design will be optimized by modifying the geometry to enhance performance and the entire process will be documented with images, calculations, and insights. I will reflect on key engineering lessons learned and time spent to complete this assignment.

## Analyze

### Design 1

#### Coarse Mesh FEA

<img width="451" height="470" alt="ChatGPT Image Oct 25, 2026, 02_44_01 AM" src="https://github.com/user-attachments/assets/0844f00c-733b-40ad-a1b4-8dee90181232" />
<img width="628" height="622" alt="ChatGPT Image Oct 25, 2026, 02_44_24 AM" src="https://github.com/user-attachments/assets/55d96316-332a-44af-bacb-738c0024383e" />
<img width="458" height="626" alt="ChatGPT Image Oct 25, 2026, 02_44_30 AM" src="https://github.com/user-attachments/assets/c1a72b13-e967-4ccf-944e-fdd5d8930294" />

#### Medium Mesh FEA

<img width="459" height="531" alt="ChatGPT Image Oct 25, 2026, 02_44_36 AM" src="https://github.com/user-attachments/assets/984d65f4-579e-4445-aa70-6d7f03dbc069" />
<img width="454" height="602" alt="ChatGPT Image Oct 25, 2026, 02_44_42 AM" src="https://github.com/user-attachments/assets/1c69ffe3-0609-4e68-8a23-19c0bd994f20" />
<img width="441" height="438" alt="ChatGPT Image Oct 25, 2026, 02_44_47 AM" src="https://github.com/user-attachments/assets/02cb97d5-92e5-4c58-9156-3345a52da6b4" />

#### Fine Mesh FEA

<img width="414" height="500" alt="ChatGPT Image Oct 25, 2026, 02_44_53 AM" src="https://github.com/user-attachments/assets/0c208e7b-8841-4124-816f-e0fb3d11be4c" />
<img width="456" height="487" alt="ChatGPT Image Oct 25, 2026, 02_44_58 AM" src="https://github.com/user-attachments/assets/2c78d842-a19b-47f0-a467-8f3937eb00cd" />
<img width="446" height="517" alt="ChatGPT Image Oct 25, 2026, 02_45_04 AM" src="https://github.com/user-attachments/assets/6adb3b7c-6b63-4d92-890c-e328df6f0bb3" />

#### Results
<img width="351" height="184" alt="1" src="https://github.com/user-attachments/assets/536c6f50-3ab8-4438-9942-3733493b82e5" />

For Design 1, I used ASTM A36 Steel and fixed the upper portion of the bracket. I applied a 1000 N force to the lower cylindrical feature. I created three meshes with 1,295, 8,803, and 66,008 elements. The bracket had a mass of 1.31 lb.

### Design 2

#### Coarse Mesh FEA

<img width="608" height="616" alt="ChatGPT Image Oct 25, 2026, 02_35_07 AM" src="https://github.com/user-attachments/assets/1a9e7bb0-eff0-40ab-b41e-e3bfa5fdda05" />
<img width="623" height="734" alt="ChatGPT Image Oct 25, 2026, 02_35_21 AM" src="https://github.com/user-attachments/assets/e8d9761a-39ca-4e6e-a833-9a0ca7f95c53" />
<img width="623" height="607" alt="ChatGPT Image Oct 25, 2026, 02_35_29 AM" src="https://github.com/user-attachments/assets/da2a5b5c-a07d-472f-86ad-8443311b8de0" />

#### Medium Mesh FEA

<img width="622" height="610" alt="ChatGPT Image Oct 25, 2026, 02_35_37 AM" src="https://github.com/user-attachments/assets/50ecb846-62aa-4ec2-9fe1-d393d99f8380" />
<img width="619" height="664" alt="ChatGPT Image Oct 25, 2026, 02_35_44 AM" src="https://github.com/user-attachments/assets/40f04bc1-f7d3-449c-8331-ae6b76351aeb" />
<img width="627" height="625" alt="ChatGPT Image Oct 25, 2026, 02_35_51 AM" src="https://github.com/user-attachments/assets/70509994-8365-4407-9bff-7be591a6d0f3" />

#### Fine Mesh FEA

<img width="437" height="499" alt="ChatGPT Image Oct 25, 2026, 02_35_58 AM" src="https://github.com/user-attachments/assets/def35111-1249-4be3-bb7f-d58ab22a53f8" />
<img width="481" height="626" alt="ChatGPT Image Oct 25, 2026, 02_36_04 AM" src="https://github.com/user-attachments/assets/30ce00cb-bf68-4563-a22c-958a9f95d551" />
<img width="462" height="664" alt="ChatGPT Image Oct 25, 2026, 02_36_10 AM" src="https://github.com/user-attachments/assets/b9a9da65-8d69-4994-82c6-86324e56461a" />


#### Results
<img width="352" height="182" alt="2" src="https://github.com/user-attachments/assets/3717aa24-4f3c-402f-afe0-da15571ccb7f" />

For Design 2, I reduced the depth of the bracket. I used the same material, fixed constraints, and 1000 N force. I created three meshes with 1,269, 8,433, and 61,509 elements. The mass decreased to 1.16 lb.

### Design 3

#### Coarse Mesh FEA

<img width="631" height="653" alt="ChatGPT Image Oct 25, 2026, 02_39_22 AM" src="https://github.com/user-attachments/assets/c20734e3-b0cd-4a44-99b5-10207f0e957a" />
<img width="625" height="631" alt="ChatGPT Image Oct 25, 2026, 02_39_29 AM" src="https://github.com/user-attachments/assets/f247def9-6e10-4bab-bcf8-05e912736dc3" />
<img width="631" height="644" alt="ChatGPT Image Oct 25, 2026, 02_39_35 AM" src="https://github.com/user-attachments/assets/d6dccdd2-0353-42b4-bbed-f0d97829e4bf" />

#### Medium Mesh FEA

<img width="426" height="458" alt="ChatGPT Image Oct 25, 2026, 02_39_41 AM" src="https://github.com/user-attachments/assets/040b7502-f7a3-40ec-9444-ed3a6ee59d11" />
<img width="432" height="479" alt="ChatGPT Image Oct 25, 2026, 02_39_48 AM" src="https://github.com/user-attachments/assets/6b1cddee-89b5-4c44-86a7-8f3a4596be0a" />
<img width="464" height="557" alt="ChatGPT Image Oct 25, 2026, 02_39_54 AM" src="https://github.com/user-attachments/assets/e05c19d1-8449-40a6-a158-13f41efae218" />

#### Fine Mesh FEA

<img width="464" height="527" alt="ChatGPT Image Oct 25, 2026, 02_40_01 AM" src="https://github.com/user-attachments/assets/ed64a3c1-bd60-4858-b462-fe5b550b957f" />
<img width="440" height="548" alt="ChatGPT Image Oct 25, 2026, 02_40_30 AM" src="https://github.com/user-attachments/assets/ee0e43cb-91a3-4099-99c2-e6368c16c6cc" />
<img width="461" height="656" alt="ChatGPT Image Oct 25, 2026, 02_40_39 AM" src="https://github.com/user-attachments/assets/d1e22f84-910e-4cc7-b91c-041f5abe2168" />

#### Results
<img width="350" height="176" alt="3" src="https://github.com/user-attachments/assets/4f2bb151-243c-4d41-bedb-d636a51b9953" />

For Design 3, I reduced the depth of the bracket again. I kept the same material, fixed constraints, and 1000 N force. I created three meshes with 1,297, 8,819, and 63,820 elements. The mass decreased to 1.07 lb, making it the lightest design.

## Decide
### Design Comparison

<img width="377" height="206" alt="Screenshot 2026-10-25 065838" src="https://github.com/user-attachments/assets/c8712869-933c-4a4e-8994-0f7bd2efc7fb" />

Design 1 had the greatest mass at 1.31 lb. It produced the lowest maximum displacement of 0.0001742 mm and a minimum factor of safety of 237.1. 

Design 2 reduced the mass to 1.16 lb without increasing the reported maximum stress compared with Design I. Its maximum displacement increased slightly to 0.0001754 mm.

Design 3 had the lowest mass at 1.07 lb. Compared with Design I, this represents a mass reduction of approximately 18.32%. Its maximum stress increased from 1.054 MPa to 1.090 MPa, while its minimum factor of safety decreased from 237.1 to 229.5.

All three designs had maximum stresses far below the 250 MPa yield strength of ASTM A36 Steel under the simulated 1000 N loading condition.

### Mesh Convergence Calculations
<img width="353" height="463" alt="Screenshot 2026-10-25 055357" src="https://github.com/user-attachments/assets/050d4ca9-7017-4093-857b-134164393dd8" />

For the convergence I used the medium and fine mesh for the most accurate results. The maximum displacement converged within 7% for all three designs. However, the maximum stress and minimum factor of safety did not converge within the required tolerance. The fine mesh results were used for the final comparison since convergence was not achieved after three attempts. After design 1 I decided to decrease the depth of the upper part of the bracket from 1.15 in to 1 in in to lower the mass, this ended up decreasing the max stress and the minimum factor of safety. I then decreased the depth of the upper part of the bracket from 1 in to .90 in to further lower the mass and this increased the max stress and the minimum factor of safety. Design 2 produced the results closest to the 7% mesh convergence requirement, though design 3 was the most lightweight and design 1 was the strongest and stiffest.

## Communicate
### Lessons learned
I learned how to use FEA to evaluate and improve my bracket design by using mesh convergence. By changing the depth of the bracket, I was able to reduce its mass and learn how changes in geometry affect its strength and stiffness. I also learned how to analyze maximum stress, displacement, and factor of safety. 

### Mistakes
One mistake I made was applying fixed constraints to the entire bracket when only the upper portion should have been fixed. I corrected this by drawing a horizontal line above the cylindrical portion and using the Split feature to separate the fixed region from the rest of the bracket.

I spent approximately 4 hours on this assignment.

[Download CAD File](https://raw.githubusercontent.com/dchouffani/megr2156-portfolio/main/docs/assignments/A07/A7%20Bracket%20Design.SLDPRT)
