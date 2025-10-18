# DAY-5 CMOS POWER SUPPLY DEVICE VARIATION ROBUSTNESS EVALUTION
## 1.CMOS inverter robustness and powersupply variation :
> static behavior of a CMOS inverter by analyzing the effects of Power Supply Scaling.Using SPICE simulation, the inverter's characteristics are compared at different supply voltages (Vdd). The simulation sweeps Vdd from an initial value of 2.5V down in 0.5V steps. Throughout this analysis, the transistor sizes are kept constant (Wp=0.9375u and Wn=0.375u).

The simulation results reveal two main advantages and one primary disadvantage of scaling down Vdd.

### Advantages

> Increase in Gain: As the supply voltage is reduced, the inverter's voltage transfer curve (VTC) becomes much steeper, indicating a significant increase in gain."56% improvement in gain" .

> Significant Reduction in Energy: Power supply scaling provides a dramatic reduction in energy consumption. This is because switching energy is proportional to the square of the voltage (Energy=1/2CV^2).
> A "96% energy reduction" when operating at 0.5V (compared to the original 2.5V).


### Disadvantages

> Performance Impact (Increased Delay): The main drawback of lowering the supply voltage is a negative impact on performance. Transient analysis graphs show that as Vdd decreases, the rise and fall delays of the inverter increase significantly. The circuit becomes slower.


#### Conclusion:
Power supply scaling is a highly effective technique for improving the gain and dramatically reducing the energy consumption of a CMOS inverter. The energy savings are particularly significant due to their quadratic relationship with the supply voltage (V^2). 

This technique presents a critical trade-off: lowering Vdd degrades performance by increasing the circuit's switching delays. Therefore, a designer must balance the need for low power and high gain against the speed requirements of the circuit.
## Lab Observations:
<img width="1273" height="825" alt="Screenshot 2025-10-17 130705" src="https://github.com/user-attachments/assets/8256e896-323d-41f9-9e11-92c80a6ee88d" />

<img width="1269" height="822" alt="Screenshot 2025-10-17 130756" src="https://github.com/user-attachments/assets/24e9a1da-5030-4832-95d4-59136334e790" />

<img width="306" height="123" alt="gainday5" src="https://github.com/user-attachments/assets/c2c07201-9c72-4236-9361-46f7a0e0419a" />

## 2.CMOS-inverter Robustness :
In digital electronics, robustness refers to a circuit's ability to operate correctly and reliably despite "noise" and variations in its operating environment. For a CMOS inverter, this means its ability to correctly interpret a "low" input as logic '0' and a "high" input as logic '1', and in turn produce a clean, unambiguous high or low output, even in the presence of voltage fluctuations, temperature changes, and manufacturing variations.

A robust inverter has a high tolerance for noise. This robustness is primarily defined by two key static parameters: the Noise Margins and the Switching Threshold (Gain).

#### The Key Design Trade-Offs for Robustness
A designer can control robustness using two main levers: transistor sizing and power supply voltage. Both involve critical trade-offs.
> Trade-Off 1: Transistor Sizing (Robustness vs. Speed & Area)

> Trade-Off 2: Power Supply Scaling (Power vs. Robustness & Speed)
## conclusion:
The robustness of a CMOS inverter is a measure of its resilience to noise, primarily quantified by its noise margins. Achieving maximum robustness involves a fundamental design compromise.
## lab obeservations:

<img width="1271" height="818" alt="Screenshot 2025-10-17 131048" src="https://github.com/user-attachments/assets/8efd7e2a-1171-4083-8075-ec94bc4da396" />

<img width="1277" height="830" alt="Screenshot 2025-10-17 131209" src="https://github.com/user-attachments/assets/e83a64f8-1425-4fd4-8d15-15a11eb947c5" />
