# A11 – Motor Selection

## Objective


## Analyze
### Motor Selection and Attachments

<img width="353" height="240" alt="Screenshot 2026-11-22 134010" src="https://github.com/user-attachments/assets/3423ce09-2e0c-4816-8be7-b70c03ebcd67" />

The selected motor is a McMaster-Carr #6470K71 DC gearmotor with a rated torque of 11.299 N·m and a rated speed of 30 RPM. The required torque, including a safety factor of 4, is 4.9256 N·m. Since the motor's rated torque exceeds the required torque, the motor satisfies the calculated torque requirement for the maximum 2 kN load.

<img width="715" height="465" alt="Screenshot 2026-11-22 134055" src="https://github.com/user-attachments/assets/f5f57ca4-8839-4e13-8523-193808169e36" />

The torque-speed curve shows the relationship between the motor's output torque and rotational speed at 90 V DC. The graph shows approximately 200 in·lbf of torque from 0 to 26 RPM, after which the torque decreases as speed increases. The required operating speed range of 0.4724–23.6217 RPM falls within this region. 

<img width="350" height="484" alt="Screenshot 2026-11-22 174756" src="https://github.com/user-attachments/assets/aa79dd9f-a091-4946-97dd-62701581b2ab" />

I calculated the reaction force at each mounting bolt and used bearing stress to determine the minimum bracket thickness of 0.2194 mm. I selected a 4 mm thick 6061-T6 aluminum bracket to provide additional strength and stiffness.

<img width="338" height="485" alt="Screenshot 2026-11-22 175347" src="https://github.com/user-attachments/assets/47a3384f-40cb-4b95-849d-baa3610aa1fd" />

I selected a 13 mm inner diameter to provide clearance for the 12.7 mm motor shaft. I calculated an allowable shear stress of 34.76 MPa and used torsional shear stress to determine a minimum outer diameter of 15.23 mm and a minimum wall thickness of 1.11 mm.

## Decide
_Reference your concept selection (Pugh matrix) here. How does this design follow from that decision?_

## Communicate
