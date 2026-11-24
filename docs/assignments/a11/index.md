# A11 – Motor Selection

## Objective

The objective of this assignment is to select a motor, design motor mounts, and select or design a coupler for the tensile tester. The assignment also involves designing a frame to support the crosshead and tensile load, analyzing and designing clamps, creating a complete CAD model, and developing a bill of materials with engineering costs. Additionally, the assignment requires documenting any mistakes made throughout the design process, recording the actual time spent completing the project from start to finish, and including a Lessons Learned section.

## Analyze
### Motor Selection and Attachments - Dina Chouffani

<img width="353" height="240" alt="Screenshot 2026-11-22 134010" src="https://github.com/user-attachments/assets/3423ce09-2e0c-4816-8be7-b70c03ebcd67" />
<img width="745" height="528" alt="Screenshot 2026-11-22 231914" src="https://github.com/user-attachments/assets/4486225a-90af-4d50-8ae1-974ad0dab4cf" />

The selected motor is a McMaster-Carr #6470K71 DC gearmotor with a rated torque of 11.299 N·m and a rated speed of 30 RPM. The required torque, including a safety factor of 4, is 4.9256 N·m. Since the motor's rated torque exceeds the required torque, the motor satisfies the calculated torque requirement for the maximum 2 kN load.

<img width="715" height="465" alt="Screenshot 2026-11-22 134055" src="https://github.com/user-attachments/assets/f5f57ca4-8839-4e13-8523-193808169e36" />

The torque-speed curve shows the relationship between the motor's output torque and rotational speed at 90 V DC. The graph shows approximately 200 in·lbf of torque from 0 to 26 RPM, after which the torque decreases as speed increases. The required operating speed range of 0.4724–23.6217 RPM falls within this region. 

<img width="350" height="484" alt="Screenshot 2026-11-22 174756" src="https://github.com/user-attachments/assets/aa79dd9f-a091-4946-97dd-62701581b2ab" />

I calculated the reaction force at each mounting bolt and used bearing stress to determine the minimum bracket thickness of 0.2194 mm. I selected a 4 mm thick 6061-T6 aluminum bracket to provide additional strength and stiffness.

<img width="338" height="485" alt="Screenshot 2026-11-22 175347" src="https://github.com/user-attachments/assets/47a3384f-40cb-4b95-849d-baa3610aa1fd" />

I selected a 13 mm inner diameter to provide clearance for the 12.7 mm motor shaft. I calculated an allowable shear stress of 34.76 MPa and used torsional shear stress to determine a minimum outer diameter of 15.23 mm and a minimum wall thickness of 1.11 mm.

### Analyze and design a frame

<img width="341" height="437" alt="Screenshot 2026-11-22 232954" src="https://github.com/user-attachments/assets/64a47716-326e-4792-a434-972ed4530aeb" />

<img width="724" height="298" alt="Screenshot 2026-11-22 232552" src="https://github.com/user-attachments/assets/5f517466-afa9-4a79-bc7a-6d153f37aedd" />

I analyzed the motor torque acting on the top frame and calculated a reaction force of 62.77 N at each end. Using a safety factor of 4, I determined a design force of 251.08 N and a bolt shear stress of 1.25 MPa. I selected the Grainger 5JRP7 inside-corner bracket with M8 class 4.6 steel bolts. The calculated bolt shear stress was below the allowable shear stress of 34.62 MPa, indicating that the bolts are sufficient for the assumed loading.

### Bill of Materials and Labor Costs


## Frame Analysis and Design
Prior to modifying the previous design, I needed to evaluate the allowable stress acting on the frame from motor torque. To achieve this, I outlined the given parameters and variables, then sketched a free-body diagram (FBD) mapping out the combined forces on the structure. My assumptions specified that the assembly would use M5 screws sourced from Grainger. Based on a shear stress analysis, the acceptable stress limits were determined to range from 50.93 MPa to 278.07 MPa.


<img width="3023" height="1192" alt="IMG_0899" src="https://github.com/user-attachments/assets/298e9056-5f8f-46fa-95e7-cf7218a171cf" />


## Frame FEA

Prior to initiating the simulation, I attached the wide corner brackets from Grainger to the frame, leaving out the individual screws because modeling each fastener was overly tedious. By applying a 2 kN load to the upper crossbar and setting fixed constraints on the lower legs, I executed a three-step mesh study.

Although the deflection values converged successfully, the stress levels failed to converge and vastly exceeded the maximum allowable threshold. The exceptionally high stress resulted from the missing fasteners, whereas the convergence difficulties were triggered by the bracket's sharp internal corners. We could resolve this by incorporating corner fillets or adding a central reinforcement web to the bracket. As another option we could weld the frame assembly together using a TIG welding procedure or a MIG setup equipped with an aluminum spool torch.

<img width="539" height="353" alt="image" src="https://github.com/user-attachments/assets/416a0403-25c4-44f4-ac3d-31fff27126c4" />


<img width="526" height="356" alt="image" src="https://github.com/user-attachments/assets/ec95b312-3594-4c38-9bdc-09c2d2e7ed30" />


<img width="3021" height="2569" alt="IMG_0897" src="https://github.com/user-attachments/assets/0e1b0ead-9ed7-4e6e-a445-af512be51d26" />



### Design Floating Bearing Mount
For the bearing mount design requiring an RC3 fit, I consulted the Machinery's Handbook. By referencing Table 8a on page 654, I established the known outer diameter and required tolerances. Afterward, I sketched a free-body diagram and applied torque analysis equations to calculate the appropriate inner wall thickness and diameter.

<img width="3021" height="1386" alt="IMG_0898" src="https://github.com/user-attachments/assets/7deb4ca3-da70-4d4f-949e-55c8ae074760" />


<img width="284" height="279" alt="image" src="https://github.com/user-attachments/assets/531033ca-a4f9-40a6-9c55-2c1e27f492ff" />


<img width="352" height="256" alt="image" src="https://github.com/user-attachments/assets/ebdd1589-c109-404b-a44b-299548e85669" />


## Bill of Materials

| Item # | Quantity | Name | Cost/Item | Cost | Purchase Link |
|:---:|:---:|---|---:|---:|---|
| 804T48 | 1 | 40 Series T-Slot Aluminum Framing, 80 mm × 40 mm, 3 m Long | $245.87 | $245.87 | [Grainger](https://www.grainger.com/search?searchQuery=804T48) |
| 95120A592 | 2 | 932 Bearing Bronze ACME Flange Nut, 3/8"-12 RH | $111.78 | $223.56 | [McMaster-Carr](https://www.mcmaster.com/95120A592) |
| 98935A817 | 2 | Carbon Steel ACME Lead Screw, 3/8"-12 RH, 36" Long | $10.15 | $20.30 | [McMaster-Carr](https://www.mcmaster.com/98935A817/) |
| 3333_0 | 2 | NEMA 23 Stepper Motor | $72.00 | $144.00 | [Phidgets](https://www.phidgets.com/?prodid=352#Tab_Downloads) |
| 5JRU7 | 6 | Wide Inside-Corner Bracket | $10.92 | $65.52 | [Grainger](https://www.grainger.com/product/80-20-Inside-Corner-Bracket-Wide-5JRU7) |
| 55MT26 | 24 | Hammer Nut | $3.50 | $21.00 | [Grainger](https://www.grainger.com/product/FATH-INC-Hammer-Nut-M5-Size-55MT26) |
| 3613N15 | 2 | Set Screw Shaft Coupling | $74.49 | $148.98 | [McMaster-Carr](https://www.mcmaster.com/3613N15/) |
| | | | **Total Cost** | **$869.23** | |


## Labor Cost
| Person | Hours Worked | Cost/Hour | Cost |
|---|:---:|:---:|---:|
| All Members | 16 hrs | $35/hr | $560 |

## Total Cost
1,429.23

## Final Design
Following the cost tabulation and finite element analysis (FEA), I finalized the design and constructed the tensile tester. To mitigate high stress concentrations and improve structural rigidity, I integrated wide brackets and hammer nuts at the corners, while also building additional support legs from leftover T-slot framing to ensure stability during loading.

<img width="266" height="432" alt="image" src="https://github.com/user-attachments/assets/f702a44f-a2d3-43c0-a23e-f087cc7b10b8" />



### Lessons Learned

We learned how to select the right motor using torque and speed requirements from the leadscrew design and how to design a motor mount bracket to attach the motor to the tester frame while maintaining precise alignment with the leadscrew, accommodating service access for assembly and maintenance, and withstanding operational torque and reaction forces without excessive deflection. We also learned how to select and design a coupler using shear stress torsion analysis and how to select proper connectors for T-slot framing by analyzing the twist caused by the motors. Additionally, we learned how to use FEA to verify that the top of the frame provides enough strength to withstand the leadscrew load and torque. Finally, we learned how to design a mounting bearing that allows the end of the leadscrew to rotate using an RC3 fit class and attaches to the bottom of the frame.

## CAD Files

[assemblymotor.zip](https://github.com/user-attachments/files/35308078/assemblymotor.zip)

