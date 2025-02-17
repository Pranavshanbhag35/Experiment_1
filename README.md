# Experiment_1
## Design 1: Simulation of CS Amplifier
## Aim 
Simulate the DC analysis, Transient, and AC analysis of a CS amplifier circuit using LTSpice.
## Circuit
![image](https://github.com/user-attachments/assets/8c2fbc0b-1bf5-4585-bc45-e54a0f52082a)
## Calculation
Power Calculation P = 100 uW
Drain Equation VDD = VDS + Vrd.
VDD = VDS + id*rd
Vds=Vdd-id*rd
P = I*V
Therefore ID = 55.5 uA
Length= 265 um   Width=480 um
Therfore VDS = Vout
VDS=1.74 V
Q point is (1.74v V,55.55 uA)
## Procedure:
1.	Make the circuit connection as show above.
2.	Apply the DC voltage of VDD = 1.8 V and VGS = 0.9 V.
3.	Set the width and Lenth of mosfet by calculation.
4.	For DC Analysis, In simulate option. Click on DC Analysis then Run the simulation.
5.	Determine the ID=55.5uA and operating point.
6.	For Transient Analysis, Change the voltage source VGS to sine wave with Dc level is 0.9v, Amplitude is 50mV, frequency is 1 kHz, In simulate option set stop time as 5ms & simulate it.
7.	For AC Analysis, In simulate option Select Ac Analysis option set points per Decade to 10, Frequency ranges from 0.1Hz to 1THz. 
8.	Simulate it & determine the gain and frequency response of the circuit.
## Result
**1.DC Analysis:**

![image](https://github.com/user-attachments/assets/528326e2-4fcc-4c26-a2a8-93d660bbc9e5)

ID=55.5uA Vout=1.74v W=480u L=265u

**Transient Analysis:**
![image](https://github.com/user-attachments/assets/f15b50a2-31b0-4ea4-8883-4613baef9981)

There is 180-degree phase shift between input and output.

**AC Analysis:**
![image](https://github.com/user-attachments/assets/075b31d9-21c1-45ff-b0a2-4db33c4f8b51)

Gain=2.3 dB

## Inference
1.	If the width of the mosfet increases then the Drain Current ID will be increased. Therefore, drain current is directly proportional to the channel width W.
2.	If the length of the mosfet increases then the Drain Current ID will be decreased. Therefore, drain current is indirectly proportional to the channel length L.
3.	If the Overdrive Voltage increases then the Drain Current ID will be decreased. Therefore, drain current is directly proportional to the Overdrive voltage Vov.
4.	180-degree phase shift between the input and output waveform.

## Design 2: Simulation of CMOS Amplifier
## Aim
Simulate the DC analysis, Transient, and AC analysis of a CMOS amplifier circuit using LTSpice.
## circuit
![image](https://github.com/user-attachments/assets/afebf698-5a7a-4a4a-9e4f-423c9fc2401d)

## procedure
1.	Make the circuit connection as show above.
2.	Apply the DC voltage of VDD = 1.8 V
3.	Set the Length as constant and determine the Width or vice versa.
4.	For DC sweep Analysis, In simulate option select DC sweep option and choose
Source name= Vin. -type of Sweep= Linear. -start value=0, -stop value =VDD=1.8 V. -increment=0.1. & find the Vin from the vtc curve.
5.  For DC Analysis, in simulate option select DC Analysis simulate and determine operating voltage of Mosfet.
6.  For Transient Analysis make DC level as 0.9v Amplitude as50mV and frequency as 1kHz and set the stop time as 5mS.
7.  for Ac Analysis Set the Type of Sweep to Decade.Set Points per Decade to 10.Set the Frequency Range from 0.1 Hz to 1 THz.Click OK. Determine the gain and frequency response of the circuit.
## Result
**DC Sweep Analysis:**
![image](https://github.com/user-attachments/assets/c25c34dd-cc29-44f3-bfec-58c69b21ee4b) 

the value of the Vin is selected as 0.8V as it is present in the middle of the saturation region of the VTC Curve.
**DC Analysis:**
![image](https://github.com/user-attachments/assets/9c459922-4409-4f35-97b7-b585c0c14fc8)

drain current Id=55.55 uA Vout=1.22 V
Length M1= 180 nm,Width=190 nm for M1.
Length M2= 240 nm,Width=480 um for M2

**Transient Analysis:**
![image](https://github.com/user-attachments/assets/c20177b5-fd60-4d47-bfc4-d871fc72e723)

There is 180 degree phase shift between input and output

**AC Analysis:**
![image](https://github.com/user-attachments/assets/615bb347-2062-4563-a3ae-9eea45252073)

## Inference
1.	If the width of the mosfet increases then the Drain Current ID will be increased. Therefore, drain current is directly proportional to the channel width W.
2.	If the length of the mosfet increases then the Drain Current ID will be decreased. Therefore, drain current is indirectly proportional to the channel length L.

3.If width is increased it leads to a higher gain

4.180 degree phase shift between the input and output waveform.


