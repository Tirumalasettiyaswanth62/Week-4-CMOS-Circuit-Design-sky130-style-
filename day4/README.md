# DAY-4 NOICE-MARGINS
## The ideal inverter I/O characteristic with the actual (realistic) characteristic.
> An ideal inverter has an "infinite slope" , meaning its output switches instantly from high (Vdd) to low (0) as the input (Vin) crosses a single threshold, Vdd/2.
> An actual inverter has a finite slope, meaning there is a transition region rather than a sharp switch.
To define the operating regions of an actual inverter, several key voltage points are established. These points are formally defined where the slope of the voltage transfer curve (Vout vs. Vin ) equals -1.

> Vil (Input Low Voltage): The maximum input voltage that is still recognized as a logic '0'.
> Vih (Input High Voltage): The minimum input voltage that is recognized as a logic '1'.
> Vol (Output Low Voltage): The output voltage when the input is Vih.
> Voh (Output High Voltage): The output voltage when the input is Vil.
### From these definitions, the two noise margins are calculated:
#### Noise Margin Low (NM_l): This margin defines the tolerance for a 'low' signal. 
> It is calculated as NM_l = Vil - Vol.
#### Noise Margin High (NM_h): This margin defines the tolerance for a 'high' signal. 
> It is calculated as NM_h = Voh - Vih.
#### The region between Vil and Vil is known as the "Undefined Region".  
Any input signal that falls into this range will produce an "indefinite logic level". 
> NM_h and NM_l values are dependent on the transistor sizing ratios (W/L) of the CMOS inverter.
## Labs outputs:
<img width="1274" height="817" alt="day4noisemargincode" src="https://github.com/user-attachments/assets/4929536b-5cb5-450f-b0b1-1bd2623ac2b9" />

<img width="297" height="91" alt="noise marhin high-low" src="https://github.com/user-attachments/assets/2a52514e-a652-4e06-8cf7-c33e39f5185c" />

<img width="1278" height="829" alt="Screenshot 2025-10-15 194916" src="https://github.com/user-attachments/assets/6c58382d-f01d-415b-bc46-265b544302c8" />


## Conclusion:

The noise margins, NM_h and NM_l, are critical metrics for determining the robustness of a CMOS inverter against voltage noise18. They quantify the "buffer" zones a logic signal has before it risks being misinterpreted.For reliable operation, a logic '0' signal must remain below Vil and a logic '1' signal must remain above Vih. If noise causes a signal to enter the "Undefined Region" (between V_il and Vih), the inverter's output becomes unpredictable. Therefore, designing inverters with larger noise margins is essential for ensuring the stability and reliability of digital circuits.
