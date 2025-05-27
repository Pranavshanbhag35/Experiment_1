# Folded Cascode OTA
## Introduction
Operational Transconductance Amplifiers (OTAs) are essential parts of analog circuit design and are frequently found in signal processing systems, filters, and analog-to-digital converters (ADCs). With its small single-stage design, high gain, and wide output swing, the Folded Cascode OTA is unique among OTA architectures. By folding the input differential pair's current path through a complementary branch, the folded cascode topology increases headroom in contrast to traditional cascode amplifiers, which have limited voltage swing because of stacked transistors. The design, theoretical analysis, and simulation of a Folded Cascode OTA are presented in this paper. Using LTspice, DC, AC, transient, and noise simulations show the benefits of this design in terms of performance. The outcomes verify that the folded cascode design attains a superior trade-off.

## Working Methodology
The folded cascode operational transconductance amplifier (OTA) implemented in this design achieves high gain and improved voltage swing through a combination of differential input processing and cascode current mirroring. The input stage comprises NMOS transistors (M9 and M10) configured as a differential pair, with a constant bias current provided by the NMOS transistor M11 acting as a tail current source. The differential voltage applied between the gates of M9 and M10 modulates the distribution of this bias current. The resulting currents are directed upward through NMOS cascode transistors (M6 and M5) and folded into the drains of PMOS transistors (M4 and M3), which transfer the signal to the upper half of the circuit. The PMOS transistors M1 and M2 form a cascode current mirror that senses these variations and generates a single-ended output voltage at the node Vout.
To enhance gain, NMOS cascode devices (M6–M8) are used to increase the output impedance. Bias voltages Vb, Vc, and Vd are applied to maintain all       MOSFETs in saturation, ensuring linear operation and optimal transconductance. Vb sets the operating point for the PMOS cascode devices, Vc biases the NMOS cascode transistors, and Vd establishes the current in the differential pair's tail source. Additionally, a load capacitor C1 at the output node introduces a dominant pole, defining the amplifier's bandwidth and contributing to its frequency stability. This folded cascode configuration enables a wide input/output voltage swing and high DC gain while maintaining power efficiency, making it highly suitable for low-voltage, high-speed analog applications.

## Circuit Diagram
![image](https://github.com/user-attachments/assets/a485c8b6-4150-4b17-a84b-9ca720d3f678)

## Technical Specification
•	Voltage Gain (Av): 60–75 dB .



•	Unity Gain Bandwidth (UGB): ~80 MHz




•	Power Consumption: ~36 µW .




•	Load Capacitance: 0.1 pF – 1 pF (external compensation capacitor).





•	Input-Referred Offset Voltage: < 5 mV .





•	Common-Mode Rejection Ratio (CMRR): > 60 dB .





•	Power Supply Rejection Ratio: > 60 dB .





•	Noise Performance: Input-referred noise dominated by M9/M10 pair.

## Advantages
•	High Voltage Gain




•	Wide Bandwidth



•	Stable Operation



•	Low Power Consumption



•	Low Noise




•	Low Offset Voltage




•	Good Common-Mode and Power Supply Rejection




•	Compact Load Capacitance Range




## Simulation Result
Input wave
![image](https://github.com/user-attachments/assets/2080b442-8361-4bdb-80bf-20ecc91faa26)



Transient Analysis output:
![image](https://github.com/user-attachments/assets/c104e30e-0e3a-4287-8948-206b5c3a12b6)




DC Analysis Output: 
![image](https://github.com/user-attachments/assets/cf92a448-c275-4c32-a094-4533e3b1b470)



Ac Analysis Output:
![image](https://github.com/user-attachments/assets/10b53ec5-6666-4390-bcab-f657e07f5052)

## Inference
The folded cascode OTA described offers  excellent performance with high voltage gain, wide bandwidth, and stability, making it ideal for low-power, precision applications. Its low noise, minimal offset voltage, and strong immunity to common-mode and power supply noise enhance its reliability and accuracy. The flexibility in handling different load capacitances and the efficient power consumption further make it suitable for integrated circuit designs that require high performance and low energy usage

## Conclusion
The folded cascode OTA with the specified characteristics provides a robust solution for high-gain, low-noise amplification in applications requiring precise signal processing. Its low power consumption, high bandwidth, and stability across varying load capacitances make it an ideal choice for energy-efficient integrated circuits. The low offset voltage and strong rejection of common-mode and power supply noise further enhance its reliability, ensuring accurate and consistent performance in practical scenarios.

## REFERENCE
•	HTTPS://PEOPLE.ENGR.TAMU.EDU/SPALERMO/ECEN474/LECTURE14_EE474_FOLDED_CASCODE_OTA.PDF


•	HTTPS://IEEEXPLORE.IEEE.ORG/DOCUMENT/1708674


•	HTTPS://SCISPACE.COM/PDF/DESIGN-OF-FOLDED-CASCODE-OTA-IN-DIFFERENT-REGIONS-OF-1F6AFIH0I4.PDF



•	HTTPS://WWW.IJERA.COM/PAPERS/VOL2_ISSUE1/CM21566570.PDF

## 9. Contributors

- Pranav Maruti Shanbhag (USN: 4NI24EC407)
- Adithya Y (USN: 4N23EC005)  
