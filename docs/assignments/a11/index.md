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

## Decide
### Design Floating Bearing Mount

## Communicate

### Lessons Learned

We learned how to select the right motor using torque and speed requirements from the leadscrew design and how to design a motor mount bracket to attach the motor to the tester frame while maintaining precise alignment with the leadscrew, accommodating service access for assembly and maintenance, and withstanding operational torque and reaction forces without excessive deflection. We also learned how to select and design a coupler using shear stress torsion analysis and how to select proper connectors for T-slot framing by analyzing the twist caused by the motors. Additionally, we learned how to use FEA to verify that the top of the frame provides enough strength to withstand the leadscrew load and torque. Finally, we learned how to design a mounting bearing that allows the end of the leadscrew to rotate using an RC3 fit class and attaches to the bottom of the frame.
