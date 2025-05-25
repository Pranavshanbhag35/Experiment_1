# Monostable multivibrator
## Aim
### Generate pulse of width 0.5ms using 555 timer IC.
## Theory
Monostable multivibrators have only one stable state that is used to generate a single o/p pulse of a specified width either high or low when an external trigger pulse is applied. This trigger pulse starts a timing cycle, which causes the o/p to change its state at the time of start of timing cycle and continues in the second state which is decided by the time constant of the capacitor C and resistor R until it returns to its original state. It will continue in this state until another i/p signal is received. Monostable multivibrators can produce a much longer rectangular waveform. When a trigger pulse is applied externally then the leading edge of the waveform rises with the externally applied trigger. Here, trailing edge depends upon the RC time constant of the feedback components used. This RC time constant may be varied with time to produce a series of pulses which have a fixed time delay to the original triggered pulse.
## Working
The output of the monostable multivibrator using 555 timer remains in its stable state until it gets a trigger. In monostable 555 multivibrator, when both the transistor and capacitor are shorted then this state is called as a stable state. When the voltage goes below at the second pin of the 555 IC, the o/p becomes high. This high state is called quasi stable state. When the circuit activates then the transition from a stable state to quasi stable state. Then the discharge transistor is cut off and capacitor starts charging to VCC. Charging of the capacitor is done via the resistor R1 with a time constant R1C1. Hence, the voltage of the capacitor increases and finally exceeds 2/3 Vcc, it will change the internal control flip flop, thereby turning off the 555 timer IC. Thus the o/p goes back to its stable state from an unstable state.
The Time duration of the pulse is given by
T = 1.1RC
Where, R is in Ω and C in Farads.
Finally we can conclude that, in the monostable multivibrator using 555 timer, the o/p stays in a low state until it gets a trigger i/p. This type of operation is used in push to operate systems. When the input is triggered, then the o/p will go to high state & comes back to its original state.
## Circuit Diagram
![image](https://github.com/user-attachments/assets/f09d2014-f234-4cf1-947f-79f882f99862)
## Calculation
Given that T=0.5ms and assume c=1uF.

T=1.1RC
R =  0.5mS/(1.1×1uF) = 454.54 Ohm.
## Procedure
1.	Build the circuit as per the Circuit diagram.
2.	Calculate the resistor R and capacitor C using the formula ton=1.1RC.
3.	In simulation we used signal generator for triggering the circuit. 
4.	Analyze the capacitor charging and discharging Voltage per time.
5.	Analyze the ton period when input is triggered. 
## Output Waveform
![image](https://github.com/user-attachments/assets/141243cc-a94a-4485-b145-532742e47138)

First waveform is triggering pulse for Monostable Multivibrator, Second waveform is Voltage across the Capacitor and Third waveform is output Pulse of 0.5ms
## Inference
•	The output of the circuit remains LOW in its stable state until a trigger input is applied.

•	Upon receiving the trigger, the output switches to HIGH and stays in that state for a time period determined by the RC time constant.

•	With the capacitor value chosen as 1 µF, the required resistor value was calculated to be approximately 454.54 Ω to achieve a 0.5 ms pulse.

•	This experiment demonstrates the use of a 555 timer in monostable mode for generating precise time delays.

## Conculsion
The 555 timer IC in monostable mode successfully generated a 0.5 ms output pulse in response to a trigger input. The output pulse duration matched the calculated value using the formula T = 1.1 × R × C, demonstrating the timer’s effectiveness in generating precise time delays.


## Aim
## Generate pulse of width 0.5ms using 555 timer IC.
## Theory
A astable multivibrator, often called a free-running multivibrator, is a rectangular-wave generating circuit. Unlike the monostable multivibrator this circuit does not require any external triggering to change the state of the output, hence the name free-running. However, the time during which the output is either high or low is determined by the two resistors and a capacitor, which are externally connected to the 555 timers.
In the differentiator amplifier circuit, the position of the capacitor and resistor have been reversed and now the reactance, XC is connected to the input terminal of the inverting amplifier while the resistor, Rƒ forms the negative feedback element across the operational amplifier as normal.
This operational amplifier circuit performs the mathematical operation of Differentiation. In other words the faster or larger the change to the input voltage signal, the greater the input current, the greater will be the output voltage change in response, becoming more of a “spike” in shape.
As with the integrator circuit, we have a resistor and capacitor forming an RC Network across the operational amplifier and the reactance ( Xc ) of the capacitor plays a major role in the performance of a Op-amp Differentiator.
Clipper is used clip the positive spikes and clipper circuit output will trigger the Monostable Multivibrator
Monostable multivibrators have only one stable state that is used to generate a single o/p pulse of a specified width either high or low when an external trigger pulse is applied. This trigger pulse starts a timing cycle, which causes the o/p to change its state at the time of start of timing cycle and continues in the second state which is decided by the time constant of the capacitor C and resistor R until it returns to its original state. It will continue in this state until another i/p signal is received. Monostable multivibrators can produce a much longer rectangular waveform. When a trigger pulse is applied externally then the leading edge of the waveform rises with the externally applied trigger. Here, trailing edge depends upon the RC time constant of the feedback components used. This RC time constant may be varied with time to produce a series of pulses which have a fixed time delay to the original triggered pulse.

## Procedure
1.	Build the circuit as per the Circuit diagram.
2.	Calculate the resistor R and capacitor C for Astable multivibrator Differentiator, clipper and Monostable multivibrator.
3.	Analyze the capacitor charging and discharging Voltage per time.
4.	Analyze the ton period when input is triggered.

## Circuit Diagram:
![image](https://github.com/user-attachments/assets/26366c2f-b938-4156-87b4-d271642cab11)

## Waveform
# Case 1:
![image](https://github.com/user-attachments/assets/869ae537-cf97-49a5-940f-e22fd3acb0af)

First wave is output of Astable Multivibrator, Second waveform is Output of Differentiator Circuit output, 3rd wave is the output of Positive Clipper circuit and fourth waveform is output of Monostable Multivibrator pulse width is 0.5ms.

# Case 2:
![image](https://github.com/user-attachments/assets/bb46eddd-1ef1-4312-8ae4-5ee948d2a8d7)

First wave is output of Astable Multivibrator, Second waveform is Output of Differentiator Circuit output, 3rd wave is the output of Positive Clipper circuit and fourth waveform is output of Monostable Multivibrator pulse width is 0.5ms.

# Simulation in Virtual Lab Astable Multivibrator
## Procedure:
1.	Connect the components as mentioned below: L1-L12, L14-L12, L16-L12, L4-L9, L8-L9, L10-L19, L3-L17, L11-L13, L7-L19, L6-L13, L2-L13, L5-L15, L18-L9.(For eg. click on 1 and then drag to 12 and so on.)
2.	Click on 'Check Connection' button to check the connections.
3.	If connected wrong, click on the wrong connection. Else click on 'Delete all connection' button to erase all the connections.
4.	Intially set R a=3.3 kΩ, R b=6.8kΩ, C=0.1µf, Vcc=5 V.
5.	Click on "Calculate" button.
6.	Now note the output voltage.
7.	Click on "Plot" button to plot Output Voltage, Capacitance Voltage
8.	Click on "Clear" button to clear the data.
9.	Repeat the experiment for another set of resistance value.
10.	Set the Resistance (Ra) value (1 kΩ - 10 kΩ).
11.	Set the Resistance (Rb) value (1 kΩ - 10 kΩ).
12.	Set the Capacitance (C) value (0.1 µf - 10 µf) .
13.	Set supply voltage (Vcc).

## Circuit Diagram
![image](https://github.com/user-attachments/assets/84bdd13c-5c06-4e09-a1a1-41ebcdcf4a6b)

## Otuput Waveform
Voltage Across the Capacitor: 
![image](https://github.com/user-attachments/assets/929fa028-39d0-47d6-bb2d-893dd75a726c)

Output Waveform: -
![image](https://github.com/user-attachments/assets/10f076e5-9dbc-4486-b668-c16dc3c2def0)

# Simulation in Virtual Lab Monostable Multivibrator
## Procedure:
1.	Connect the components as mentioned below: L1-L12, L14-L12, L16-L12, L4-L9, L8-L9, L9-L10, L3-L17, L11-L13, L7-L11, L6-L13, L5-L15.(For eg. click on 1 and then drag to 12 and so on.)
2.	Click on 'Check Connection' button to check the connections.
3.	If connected wrong, click on the wrong connection. Else click on 'Delete all connection' button to erase all the connections.
4.	Intially set R a=10 kΩ, C=1 µf, Vcc=5 V, Tin = 20 msec.
5.	Click on "Calculate" button.
6.	Now note the output voltage.
7.	Click on "Plot" button to plot, Trigger Input Voltage, Output Voltage, Capacitance Voltage
8.	Click on "Clear" button to clear the data.
9.	Repeat the experiment for another set of resistance value and capacitance value.
10.	Set the Resistance (R a) value (1 kΩ - 10 kΩ).
11.	Set the Capacitance (C) value .
12.	Set supply voltage (Vcc).
## Circuit Diagram
![image](https://github.com/user-attachments/assets/bcabfa8b-4c6d-4fd9-85b2-1ae949fdca52)

## Waveform
Triggering pulse input waveform:
![image](https://github.com/user-attachments/assets/1d22377a-19d1-4c3f-a5ac-73992f390170)

Voltage Across the Capacitor: 
![image](https://github.com/user-attachments/assets/786cee74-8f69-4528-b983-a9263b696e1f)

Output Waveform: 
![image](https://github.com/user-attachments/assets/8e9a313b-de9a-41da-a336-7ae45c7bbe49)






