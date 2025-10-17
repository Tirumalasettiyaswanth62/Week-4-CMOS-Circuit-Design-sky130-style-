# Basic NMOS drain current (id) and drain to source voltages (Vds)
## I. Threshold Voltage (Vt) Formation:
Initially, with a gate-source voltage (Vgs) of zero, the connections between the P-substrate and the n+ source/drain regions form two p-n junction diodes. With zero bias, these junctions are off, resulting in a high resistance between the source and drain.

### When a positive voltage is applied to the gate, the following occurs:

- Positive charges accumulate on the gate electrode, which in turn causes an accumulation of negative charges in the substrate directly beneath it.

- This process creates a depletion region under the gate as mobile positive charges are repelled.

- As Vgs  continues to increase, the semiconductor surface under the gate inverts to n-type material. This phenomenon is called strong inversion.

- The voltage at which strong inversion occurs, forming a continuous n-channel from the source to the drain, is the threshold voltage (Vt).

  Based on the provided document, here is an overview of the principles of Threshold Voltage and MOSFET operation.

## II. Body Effect on Threshold Voltage
The threshold voltage is not constant; it is influenced by the voltage between the source and the bulk (substrate), denoted as Vsb.

### Applying a positive Vsb:

​- creates an additional reverse bias between the source and the substrate.

- This increases the depletion layer width, meaning a higher gate voltage is needed to achieve strong inversion.

Based on the provided document, here is an overview of the principles of Threshold Voltage and MOSFET operation.

## III. Transistor Operation Regions
- Once the gate voltage exceeds the threshold voltage (Vgs>Vt), the transistor operates in one of two main regions, depending on the drain-source voltage (Vds).

### 1. Linear (Resistive) Region
- This region occurs when Vg>Vt and the drain-source voltage (Vds) is relatively small.

- The current is a drift current caused by the potential difference between the drain and source.

- The drain current (Id) is dependent on both Vgs and Vds

-For very small values of Vds, this equation is approximately linear, which is why it is called the linear or resistive region of operation

### 2. Saturation Region
- As Vds increases, the voltage difference between the gate and the channel decreases near the drain side.

- When Vgs−Vds≤Vt, the channel near the drain becomes "pinched off".

- At this point, the transistor enters the saturation region. Further increases in Vds do not significantly increase the drain current.

- The drain current (Id) in this region is primarily controlled by Vgs
# Lab of the Day1:

## -Vdd branch plot 
<img width="1281" height="837" alt="day1" src="https://github.com/user-attachments/assets/f22b2639-1cb5-4953-838e-435ea56a5c37" />
