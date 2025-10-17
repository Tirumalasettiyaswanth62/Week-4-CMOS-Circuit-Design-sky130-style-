# DAY2 CMOS-CIRCUIT-DESIGN-sky130 
## Velocity Saturation And Basics of CMOS Inverter VTC :
## 1.Velocity saturation effect :
> As transistors shrink in size to lower technology nodes, a phenomenon known as velocity saturation becomes increasingly prominent, significantly impacting the performance and transfer characteristics of CMOS inverters. This effect causes a deviation from the ideal square-law behavior of MOSFETs, leading to changes in the inverter's switching behavior, gain, and noise margins.
### The Phenomenon of Velocity Saturation:
> In traditional long-channel MOSFETs, the drift velocity of charge carriers (electrons or holes) in the channel is directly proportional to the lateral electric field. However, as the channel length is scaled down in modern, lower-node transistors, the electric field strength for a given supply voltage increases dramatically.Under these high electric fields, the carriers no longer speed up indefinitely. Instead, their velocity reaches a maximum limit, known as the saturation velocity. This occurs because the carriers lose energy through increased scattering with the silicon lattice.This saturation of carrier velocity has a direct impact on the drain current (Ids) of the MOSFET. In the saturation region, the drain current, which would ideally have a quadratic relationship with the gate-to-source voltage (Vgs), becomes more linearly dependent on Vgs. This is a key departure from the classical Shockley model and is often described by the alpha-power law model. The current in a velocity-saturated device is more accurately represented as being proportional to (Vgs - Vt).
### Lab observations:
<img width="1279" height="823" alt="day2" src="https://github.com/user-attachments/assets/23ec3bb7-d817-4a4c-aa6b-076be7473522" />


### CMOS Inverter Charaterstics:
A CMOS inverter consists of a PMOS and an NMOS transistor that act as switches.
> When the input voltage (Vin) is low (0V), the PMOS transistor turns ON, and the NMOS turns OFF. This creates a direct path from the power supply (Vdd) to the output, making the output voltage (Vout) high (Vdd).

> When the input voltage (Vin) is high (Vdd), the NMOS transistor turns ON, and the PMOS turns OFF. This creates a path from the output to the ground (Vss), making the output voltage (Vout) low (0V).
#### To determine the output voltage for intermediate input values and create the VTC curve, the document outlines a graphical method:
> Plot I-V Curves: The current-voltage (Ids vs. Vds) characteristics are plotted for both the NMOS and PMOS transistors for several constant input voltages (Vin).
### Lab observations :
Id vs Vgs :
<img width="1275" height="822" alt="day2 1 Id vs Vgs " src="https://github.com/user-attachments/assets/7b627622-9c9e-46c3-9711-17c3306335d4" />
