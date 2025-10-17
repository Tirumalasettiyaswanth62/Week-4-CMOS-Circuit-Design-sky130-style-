# DAY3 : CMOS-SWITCHING THRESHOLD AND DYNAMIC SIMULATIONS :
## 1.Voltage transfer characterstics :
### Spice deck simulations for CMOS inverter :
<img width="1897" height="899" alt="Screenshot 2025-10-17 135726" src="https://github.com/user-attachments/assets/e535993b-e968-4469-a9c5-e31e58ca446f" />
<img width="1829" height="753" alt="image" src="https://github.com/user-attachments/assets/0e5c155f-8dd1-43ec-ae67-1fcc1314a486" />

### Lab simulation for CMOS inverter :
<img width="1274" height="823" alt="day3 vout vs vin " src="https://github.com/user-attachments/assets/092f7d52-c5a1-47de-b04f-2edf7844305c" />

## 2.CMOS Inverter switching threshold and robustness :
> Switching Threshold (Vt)The switching threshold, Vt is a key metric for an inverter's robustness and is defined as the input voltage (Vin) where it equals the output voltage (Vout).The document demonstrates through SPICE simulations how the sizing of the NMOS and PMOS transistors (specifically their width-to-length or W/L ratios) significantly impacts Vt.Symmetrical Inverter: When the W/L ratios of the PMOS and NMOS are equal ((W/L)p = (W/L)n = 1.5), the switching threshold is approximately 0.98V or 0.99V.Asymmetrical Inverter: By increasing the width of the PMOS transistor to make it stronger ((W/L)p = 3.75 while (W/L)n = 1.5), the switching threshold shifts to a higher value, approximately 1.2V.The analysis shows that at the switching threshold, both the NMOS and PMOS transistors are in their saturation regions. The document provides the equation to calculate Vt based on the relative strengths of the transistors.

> Propagation Delay (Rise and Fall Times)The document also evaluates the impact of transistor sizing on the inverter's rise and fall delays. Due to the lower mobility of holes, the on-resistance of a PMOS transistor is about 2.5 times greater than that of an equally sized NMOS transistor6. This inherent asymmetry affects the charging and discharging times of the output capacitor.A table summarizes the trade-offs:When the PMOS and NMOS have the same size ((W/L)p = (W/L)n), the rise time (148ps) is much longer than the fall time (71ps).By increasing the width of the PMOS relative to the NMOS, the rise time decreases while the fall time increases88.A ratio of (W/L)p approx 2 times (W/L)n results in nearly equal rise (80ps) and fall (76ps) delays.
### Lab simulations :
<img width="1279" height="828" alt="day3transient" src="https://github.com/user-attachments/assets/4225a609-00e3-412c-9834-a5f7fec6f2ad" />
<img width="1274" height="799" alt="day3 out vs time vs in" src="https://github.com/user-attachments/assets/4b98057e-dcbc-4ba5-bd8e-1af01dd6f440" />
