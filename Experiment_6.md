# Current mirror Circuit
A Golden Reference Current Source is a high-precision, stable current source used in analog and mixed-signal circuit design. It provides a consistent and temperature-insensitive reference current, often serving as the foundation for biasing other circuits like amplifiers, ADCs, and voltage references.
                
**why current mirror circuit is more preferred than tail current Source in differential amplifier?**

A current mirror circuit is preferred over a simple tail current source in a differential amplifier because it provides a more stable and precise current. Unlike a resistor-based tail current source, which is affected by power supply variations and temperature changes, a current mirror maintains a constant current, improving the amplifier’s common-mode rejection ratio (CMRR) and overall performance. This stability helps in rejecting noise and ensuring the differential amplifier functions reliably under varying conditions.
Additionally, a current mirror ensures better symmetry and matching, which is essential for proper differential amplifier operation. It provides higher output resistance, making it a more ideal current source while also consuming less power compared to a resistor-based tail source. Since a simple tail current source requires a high-value resistor and high supply voltage, it results in increased power dissipation. In contrast, a current mirror circuit delivers greater precision, stability, and efficiency, making it the preferred choice in high-performance differential amplifier designs.
## Aim: - Design and analyze current mirror circuit as active load in amplifier circuit.
## Procedure: -
1.	Design the Circuit as per the circuit in fig circuit 1 and put appropriate values of the resistor and W/L value of MOSFET.
2.	For simulation in LT spice first select DC operating point simulate the circuit find current (I out) compare from Iref and note down in tabular column 1. vary the W/L and analyze the I out.
3.	For the 2nd circuit find the Iout and Iref  make connection set the W/L value analyze the Iout and Vout.
4.	for the 3rd circuit for Nmos MOSFET make 1:2 current transfer and for Pmos MOSFET make 1:1 current transfer.
## Derivation: -
![image](https://github.com/user-attachments/assets/c9d3eb17-7d82-417f-831f-709706f4e32c)
## Circuit 1: -
![image](https://github.com/user-attachments/assets/e5464bbd-930b-429b-8283-693223456057)
## Output: -
![image](https://github.com/user-attachments/assets/5cce9cfa-6a2f-480b-9f8a-aeec4b0675aa)
## Tabular Column 1: -
| I ref  | I out Expected | I out Actual | (W/L)1 | (W/L)2 | Vx     | V out  |
|--------|---------------|--------------|--------|--------|--------|--------|
| 100uA  | 100uA         | 103uA        | 1      | 1      | 1.275V | 1.696V |
| 100uA  | 100uA         | 100.6uA      | 1      | 1      | 1.437V | 1.699V |
| 100uA  | 100uA         | 100.6uA      | 1      | 1      | 1.397V | 1.699V |
| 100uA  | 200uA         | 197.504uA    | 1      | 0.5    | 1.397V | 1.602V |
| 100uA  | 100uA         | 100uA        | 1      | 1      | 1.331V | 1.669V |

### Circuit Diagram 2: -
![image](https://github.com/user-attachments/assets/7ed7fef4-7280-4aaf-acd5-7ee158f5bfce)
### Output Waveform: -
![image](https://github.com/user-attachments/assets/4025eecb-c792-458c-a830-4d6a946fc0cf)
### Tabular Column 2: -
| I ref  | I out Expected | I out Actual | (W/L)1 | (W/L)2 |
|--------|---------------|--------------|--------|--------|
| 277uA  | 277uA         | 264.3uA      | 1      | 1      |
| 277uA  | 277uA         | 270.2uA      | 1      | 1      |
| 277uA  | 277uA         | 278.3uA      | 1      | 1      |
| 277uA  | 554uA         | 529uA        | 1      | 0.5    |

## Aim: - Design the Differential amplifier using the same design specification. And perform DC analysis, transient and AC analysis.
## Calculation
![image](https://github.com/user-attachments/assets/3ef28bc6-a630-4de1-ad91-17f0bcd379d9)
## Circuit diagram
![image](https://github.com/user-attachments/assets/05fb6c88-76e2-4079-bde0-fa3caeccf51c)

## observation
### Dc Analysis
![image](https://github.com/user-attachments/assets/40980397-119a-49c5-81fd-02ae5332172e)
### Transient Analysis
![image](https://github.com/user-attachments/assets/d4fd9aac-b642-4017-8938-88d455c8d273)

There is 180-degree phase shift between input and output. 
Gain is 6.2V/V

### Ac Analysis
![image](https://github.com/user-attachments/assets/8d5ea834-e7c7-47c1-a1ee-bd811c444258)
### Infernce
1. Current mirror Circuit sstabilizes the Circuit which makes more efficiently working.
2. By using Current mirror circuit which makes the circuit to accurate.
3. The output current increases or decreases in proportion to the (W/L) ratio of the MOSFETs, confirming the theoretical operation of the current mirror circuit.
4. When the W/L ratio of the second transistor is reduced to 0.5, the output current nearly doubles.
5. The better the matching of MOSFETs, the more accurate the current mirroring. Any mismatch in threshold voltage (Vth) or channel dimensions will cause errors.
### Conclusion
​In this experiment, we explored the design and analysis of a Golden Reference Current Source and its application in differential amplifiers. The findings highlight the superiority of current mirror circuits over simple tail current sources in terms of stability, precision, and performance.
