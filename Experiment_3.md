# Experiment_2
## Aim
Design and analyze the differential amplifier for the following specification VDD=2.2V P=2.2mV Vic=1.2V
Vocm=1.25V Vp=0.4V perform DC analysis transistor analysis, frequency response and extract the parameter
## Calculation
![image](https://github.com/user-attachments/assets/3ef28bc6-a630-4de1-ad91-17f0bcd379d9)
## Procedure 
1.	Make the circuit connection as show above.
2.	Apply the DC voltage of VDD = 2.2 V and VGS = 1.2 V.
3.	Set the width and Lenth of mosfet by calculation.
4.	For DC Analysis, In simulate option. Click on DC Analysis then Run the simulation.
5.	Determine the ID<sub>1</sub>=ID<sub>2</sub>=0.5mA and operating point.
6.	For Transient Analysis, Change the voltage source VGS to sine wave with Dc level is 1.2v, Amplitude is 50mV, frequency is 1 kHz, In simulate option set stop time as 5ms & simulate it.
7.	For AC Analysis, In simulate option Select Ac Analysis option set points per Decade to 20, Frequency ranges from 0.1Hz to 1THz. 
8.	Simulate it & determine the gain and frequency response of the circuit.
## Differential Amplifier with tail Resistor
**Circuit**
![circuit 1](https://github.com/user-attachments/assets/c3982eda-b3c6-48a6-bc8b-59be0e64fd3c)
**DC Analysis**
![crcuit_1_DC](https://github.com/user-attachments/assets/1a21842a-322c-485e-a748-c637332e9f5d)
We set Q point (1.2v,0.5mA) by Set Length as 180nm and width as 6.45um

**Transient Analysis**

the output wave form across output 
![image](https://github.com/user-attachments/assets/29e6e18f-0d64-4821-aecc-99bdf5500d0e)
![image](https://github.com/user-attachments/assets/7eda1a8d-d9df-4eeb-a574-fa5ec67924d7)
There is 180-degree phase shift between input and output.

**AC Analysis**
![image](https://github.com/user-attachments/assets/8d5ea834-e7c7-47c1-a1ee-bd811c444258)
Gain is 8.636 <sup>v</sup>/<sub>v</sub>
## Differential Amplifier with Constant Current Source in tail 
**Circuit**
![image](https://github.com/user-attachments/assets/f5945e10-c06c-4845-afed-c7ea97df0d57)
**DC Analysis**
![image](https://github.com/user-attachments/assets/b2626b73-90e0-43d8-a1c6-b2edaf7b97ed)
**Transient Analysis**

the output wave form across output 
![image](https://github.com/user-attachments/assets/8bca769f-0531-4a5c-b75e-1654c6d94e56)
**AC Analysis**
![image](https://github.com/user-attachments/assets/8d5ea834-e7c7-47c1-a1ee-bd811c444258)
## Differential Amplifier with tail MOSFET
**Circuit**
![image](https://github.com/user-attachments/assets/8cc72361-110f-4187-ad6e-818f7155b786)
For Vb = Vp + Vth = 0.4 + 0.366
Tail MOSFET act as constant current source we set L=180nm and W=18.45um.

**DC Analysis**
![image](https://github.com/user-attachments/assets/8108b932-2a0d-46a3-9378-fe3afa5e6ddf)
**Transient Analysis**
![image](https://github.com/user-attachments/assets/4281ba00-5ced-4512-bb73-787ff360f8f7)
**AC Analysis**
![image](https://github.com/user-attachments/assets/8d5ea834-e7c7-47c1-a1ee-bd811c444258)
## Inference

VDD=2.2 V
Vp=0.4 V
VICM=1.2 V
VOCM=1.25 V
RD= 1.9 kohm
RSS= 400 ohm
ISS= 1 mA
ID= 0.5 mA

1.When VICM changes there is a change in the output voltage and Drain current.
2.If the input voltage is more then the minimum swing or outside the allowable swing the output wave form deforms, ie it is in triode or cutoff region.
3.If RD value changes there will be a change in the output voltage,by selecting the resistance wecan control the output voltage.
4. If Gain will incersae then Output Swing will Be decreased.

