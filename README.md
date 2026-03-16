# 7.-Design-and-Simulation-of-single-phase-inverter
## AIM
To design, simulate and analyse a single phase Inverter using MATLAB Simulink.
## APPARATUS REQUIRED
•	MATLAB
## PROCEDURE
1.	Open MATLAB and click on the icon for SIMULINK as shown below
 <img width="522" height="376" alt="image" src="https://github.com/user-attachments/assets/64e30b59-d51a-40c6-978c-09191f5b0a7f" />

Another way is to open is through START icon of MATLAB Start ⇒ Simulink ⇒ Library  browser. 

2.	Click on NEW MODEL or go to FILE ⇒ NEW ⇒ MODEL and a new blank model is created as shown below
 <img width="572" height="382" alt="image" src="https://github.com/user-attachments/assets/e0aa2cc1-47b6-44c2-93f3-848c9f3a3740" />

3.	After creating a blank model you need to open the SIMULINK component storeroom/library by going to View ⇒ Library Browser. Select SIMPOWER SYSTEMS then select Power Electronics library and by right clicking on ideal switch or MOSFET and click on add to the model will add the ideal switch/MOSFET in the blank model. 

4.	Similarly go to ELECTRICAL SOURCES ⇒ DC Voltage Source and add it to the model. Select Elements and select “SERIES RLC BRANCH” and add it to the model. Simulink do not perform simulation unless and until a measurement block is present in a system. Since we need to measure the input and output voltages and the load current. To add them select Measurement in SIMPOWER SYSTEMS and then add current measurement and voltage measurement blocks to the model. Oscilloscope is not included in SIMPOWER SYSTEMS and is present in the top most block of the left column that is SIMULINK ⇒ Sinks ⇒ Scope. Also add PWM generator from source. We can join various blocks by clicking on their edges and then drag the wire till the other connection terminal.
5.	Construct the circuit by joining them together in the form as given below
 <img width="940" height="463" alt="image" src="https://github.com/user-attachments/assets/16d8db93-b3f6-4f1a-8222-9dcf96ae487f" />

6.	Double click on series RLC branch, Select the Branch type as R and set the values for R.
7.	Double click on PWM generator, set the parameter as per the requirement.
  <img width="1117" height="473" alt="image" src="https://github.com/user-attachments/assets/30f18b06-c629-4258-bcc6-67bd8f1bc820" />
	 

8.	Before running the simulation, we have to configure the parameters. Go to Simulation ⇒ Configuration parameters as shown
 <img width="542" height="399" alt="image" src="https://github.com/user-attachments/assets/ac8e0f9e-3b11-471a-aa75-6511081081d4" />

9.	Select the ode23tb (Stiff/TR-BDF2) or ode15s (Stiff/NDS) or any suitable solver as
shown below 
 <img width="566" height="401" alt="image" src="https://github.com/user-attachments/assets/0ffddcd7-d714-452f-aa82-d91dcec30a38" />

10.	Start the simulation and Double click on scope and observe the graphs.
## Exercise 1
Design a Single Phase Inverter having the DC input supply of 100V and output resistance 1 ohm using pulse generator.

## Simulation
![Image](https://github.com/user-attachments/assets/d665408e-cbea-4ab5-9cab-c6be973973cc)
## Output
## Result
