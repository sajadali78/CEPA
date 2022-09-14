# Complex Engineering Problem Activity (CEPA)
In  this  Complex  Engineering  Problem  Activity  (CEPA)  you  will  implement  the frequency control as well as voltage control on generation side with its protection and also  shunt  compensation  on  the  load  side  with  OC  protection  under  varying  load conditions to reduce the unnecessary burden on the transmission line. 
#### Task: 
1. Identify and connect the required equipment for the said activity.
2. Ensure the safety precautions during the wiring. 
3. Initialize the system on the No-load. 
4. Analyze the operation of Synchronous Generator at no load and Full load characteristics  
5. Analyze the effect of voltage and frequency control in power system
6. Protection of Generator with OV/UV and OF/UF values 
7. Analyze the effect of voltage regulation on load side by using SCADA 
8. OC protection on load side 
####  Important Instruction to perform this task:  
1. Use MSCom Software for the data acquisition.
2. First energize the field winding then the armature winding in separately excited DC

## **Introduction:**
Frequency control, voltage control, and their respective protections are implemented on the generation side of this Complex Engineering Problem Activity (CEPA), and shunt compensation is implemented on the load side with OC protection under different load conditions. 
## **Required & Software Equipment:**
1. Synchronous Generator 
2. Separately excited DC Motor 
2. DC Power Supply 
3. Power Circuit Breakers 
4.Feeder Manager Relay 
5. OC Relay
6. Transmission Line Model 
7. Resistive Loads 
8. Inductive Loads 
9. Capacitive Loads 
10. Power Factor Meter 
11 VI Measurement Meter 
## Software Required: 
1. MsCom2 
## Safety Precautions:  
1. The circuit must be connected in accordance with the topological circuit design. No equipment should be powered up while the circuit is connected. Because a DC motor is individually excited, its field winding must never be open-circuited.  
2.Verify that the generator's RPMs are below 3000, the nominal RPMs. 
3. Ensure that there are no cables running from the synchronous generator to the DC motor close to the prime mover

## Objectives:  
1. Implement Frequency control as well as voltage control on generation side of the system 
2. Observe the shunt compensation on load side and its impact on generation side of the power system with OC protection 
3. Observe the varying load conditions and its impact on frequency control and voltage control  
## Problems and Scope of the Activity 
We attempted to compare the combined protections of voltage, frequency, and over current in both steady and fluctuating conditions in this activity involving multiple protection schemes. Nonetheless, this work was restricted to the specifics of these protection schemes; no additional safeguards were added to the power grid. The Problems faced during this activity are summarized below: 
          - If the load was switched during normal operation to simulate an      overcurrent condition, the voltage relay would trip. 
         - The circuit breaker on the generator side was tripped because of an overloaded frequency relay. 
         - When the breaker trips, the feeder manager relay interprets this as an overvoltage situation and trips the breaker on the generation side as well.
  
 ## Single Line Diagram :  
 
 The following SLD was implemented on hardware :
 
![SLD IMAGE](https://github.com/sajadali78/CEPA/blob/main/sld.PNG)

## Hardware Implementation :

![](https://github.com/sajadali78/CEPA/blob/main/hardwareimp1.PNG)

## Procedure:  
1. Ensure proper connections of the hardware. 
2. Ensure Proper Communication of Feeder Manager Relay with MsCom2 Software:

![](https://github.com/sajadali78/CEPA/blob/main/software_step1.PNG)

3. Apply the following system settings to the feeder manager relay using MsCom2
software:

![](https://github.com/sajadali78/CEPA/blob/main/software_step2.PNG)

4. Apply the function settings to choose the relay functions for voltage and
frequency control for under and over voltage condition, similarly for frequency
under and over frequency condition:

![](https://github.com/sajadali78/CEPA/blob/main/software_step3.PNG)

5. Apply the DO configuration for chosen relay functions:

![](https://github.com/sajadali78/CEPA/blob/main/software_step4.PNG)


6. Energize the field winding of the motor first and gradually increase the voltages
of Armature winding till the prime mover achieves 3000 Nominal R.P.Ms.
Note that 3000 R.P.Ms are to be maintained throughout the lab experiment for
the normal operation of synchronous generator.
7. Take observations at no load and varying load conditions for different resistive
loads and frequency and voltage conditions.

