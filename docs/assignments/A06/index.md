# A6 – Bracket Drawing

## Objective
The objective of this assignment is to generate a comprehensive solid model and a multiview engineering drawing that accurately represents my designed bracket while ensuring that all strength and stiffness requirements are met. I will use the dimensions determined from the previous assignment to create a parametrically designed solid model based on my strength and stiffness analyses. I will then generate a fully dimensioned multiview CAD drawing with engineered tolerances. I will identify an analytical equation used to drive at least one dimension in my parametric model. Then, I will identify one dimension with a tighter tolerance and one with a looser tolerance and explain how the function of each feature justifies the selected tolerance.


## Analyze

### Governing Dimensions

<img width="248" height="349" alt="Screenshot 2026-09-28 043311" src="https://github.com/user-attachments/assets/9b9e93b3-751f-4ee8-b9c2-229a7a588bba" />

For Feature A, the stress analysis governs the diameter, resulting in a diameter of 0.8709 in. For Feature B, the stress analysis governs the thickness, resulting in a thickness of 0.15099 in. For Feature C, the stress analysis governs the height, resulting in a height of 0.7044 in. For Feature D, the stress analysis governs the thickness/length, resulting in a dimension of 0.0662 in. For Feature E, the stress analysis governs the height, resulting in a height of 0.6299 in.




## Decide

### Parametric Variables and Equations

<img width="585" height="534" alt="Screenshot 2026-09-28 041826" src="https://github.com/user-attachments/assets/da344085-5b11-44bb-bc95-16224aef221d" />

These are the variables and equations that drove the dimensions of this bracket.

### Dimensions
<img width="870" height="551" alt="main dim" src="https://github.com/user-attachments/assets/3a10bf02-a107-4e07-a62a-fa121a781b48" />

<img width="500" height="223" alt="top" src="https://github.com/user-attachments/assets/f5f2938e-87e2-4245-a800-c98b8d16ffa6" />


<img width="412" height="590" alt="b" src="https://github.com/user-attachments/assets/54f7a419-6534-4db9-91ef-9dbd010e1421" />
<img width="409" height="610" alt="a" src="https://github.com/user-attachments/assets/2a96bb06-530e-4ff0-a37a-dea63724e8c4" />

### Drawing and Tolerances
<img width="420" height="242" alt="Screenshot 2026-09-28 051459" src="https://github.com/user-attachments/assets/2417d2e9-fa60-42e5-a865-628e2112f830" />

<img width="434" height="233" alt="Screenshot 2026-09-28 051549" src="https://github.com/user-attachments/assets/95adc33b-a9c9-4c2c-b698-22e6b238e994" />

<img width="374" height="481" alt="Screenshot 2026-09-28 054838" src="https://github.com/user-attachments/assets/1da6fd52-a0d0-478e-b948-dc0ce59a7ec5" />

For a and c, I used a minimum tolerance of 0 because the opening cannot be smaller than the minimum required size, or it could interfere with the mating part. For b, I used a maximum tolerance of 0 because the solid feature cannot be larger than the maximum allowable size, or it could interfere with the mating part and prevent the required clearance.


<img width="842" height="595" alt="drawing" src="https://github.com/user-attachments/assets/bfe3aff9-7ff3-43f5-b9d6-0d4d1fa4e365" />

<img width="983" height="349" alt="draw" src="https://github.com/user-attachments/assets/c44d15f6-9ebc-4557-94d2-709bbda15e77" />


## Communicate

### Final Part

<img width="388" height="625" alt="final" src="https://github.com/user-attachments/assets/8d26fdc6-b152-4f68-a6a6-e4193af7e265" />

### Parametric Design
<img width="311" height="34" alt="Screenshot 2026-09-28 045543" src="https://github.com/user-attachments/assets/18a9f87e-6dea-4a53-8451-623dcaec32b1" />

I used the strength equation to drive the diameter of Feature A, which in turn drove the width of Feature B since I assumed the two features aligned. I expressed the strength equation in terms of the radius and entered the rearranged equation directly into CAD. I then defined the diameter as twice the calculated radius. Feature B’s width was parametrically linked to Feature A’s diameter, so a change in Feature A’s diameter would automatically update the width of Feature B.

### Tolerance Selection
<img width="365" height="147" alt="Screenshot 2026-09-28 050227" src="https://github.com/user-attachments/assets/ff03aed9-b9fd-420a-985a-c29888e70b04" />

I used a looser tolerance for dimension “a” because the previous assignment stated that “a” is intended for use where accuracy is not essential. I selected an RC5 fit for this dimension. I used a tighter tolerance for dimension “b” because the previous assignment stated that “b” represents the closest fit that can be expected to run freely. I selected an RC1 fit for this dimension. Both features are mating/functional surfaces, but “b” requires a close fit, whereas “a” does not require a close fit since accuracy is not essential.

### Lessons Learned

I learned how to create tolerance fits and how to determine which analysis governs the main dimensions of each feature.

I spent approximately 4 hours creating my part on CAD and defining tolerances.

[Download SolidWorks File](blob:https://github.com/2cda7b5b-005c-487f-b777-12cd1a9b88e2)
