# Attenuation Measurement 2.5 GB & 10 GB
# Attenuation-Limited Fiber Length

## Objective
- Calculate the attenuation-limited fiber length based on the power budget equation.  
- Simulate the resulting system and verify that it meets performance objectives.

---

## Theory
The **power budget equation** states that the power budget in a transmission system must equal the sum of all power losses plus the power margin.  

The power budget is the difference between the transmitter output power and the receiver sensitivity in dBm:

<img width="994" height="468" alt="image" src="https://github.com/user-attachments/assets/28074fe1-e571-4356-bf4c-29cf212c8173" />

In this exercise, all parameters are given except the fiber length, which must be determined.  

The **receiver sensitivity** is defined as the minimum power required to achieve a BER of <img width="54" height="38" alt="image" src="https://github.com/user-attachments/assets/56f53e67-161a-4d53-ba6e-e31a3725ea43" />, corresponding to a Q factor of 6.  
- Receiver sensitivity depends on the bit rate.  
- Fiber attenuation depends on the operating wavelength.  

---

## Pre-lab Calculations
Using the power budget equation and the parameters below, determine the attenuation-limited fiber length:

- **Transmitter output power:** 0 dBm  
- **Operating wavelength:** 1550 nm  
- **Bit rate:** 2.5 Gb/s  
- **Receiver sensitivity:** -30 dBm  
- **Fiber attenuation:** 0.19 dB/km  
- **Number of connectors:** 2  
- **Loss per connector:** 0.5 dB  
- **Additional known losses:** 0 dB  
- **Power margin:** 6 dB  

---

## Layout
- The system has been created using **OptiSystem** and exported as an **OptiPerformer** file.  
- Two versions exist: one for **2.5 Gb/s** and one for **10 Gb/s**.  
- Work with the **2.5 Gb/s** version first.  
- An optical attenuator represents connector loss and system margin.  
- Adjust parameters according to the table above.  
- Dispersion and nonlinear effects in the fiber are disabled.  
- To set the receiver sensitivity to -30 dBm for 2.5 Gb/s, set the **thermal noise parameter** in the receiver to **8.97e-24 W/Hz**.  
- Visualizer components are included to obtain necessary simulation data.  

---

## Simulation
1. Run the simulation and record:
   - **Optical power levels (dBm):**
     - Both ends of fiber  
     - Receiver input  
   - **BER analysis:**
     - BER  
     - Q factor  
     - Eye diagram  

2. Set the fiber length to **125% of the calculated pre-lab value** and repeat the simulation and data recording.  

---

## Analysis and Report
Compare simulation results with pre-lab calculations and record observations.  

Your report should contain:
- **Cover Page**
  - Title of the lab  
  - Course name and number  
  - Your name  

- **Pre-lab Calculations**  
## TABULATION
<img width="1536" height="1600" alt="image" src="https://github.com/user-attachments/assets/bb6c7348-4e5d-4229-8c88-f9682648e36a" />
<img width="1600" height="889" alt="image" src="https://github.com/user-attachments/assets/1466097a-555e-4d0a-b2d7-d1b0df4f6355" />
<img width="1600" height="1065" alt="image" src="https://github.com/user-attachments/assets/b918a9c7-f7f7-4c16-8e5d-a93829e6824f" />

## GRAPH OF 2.5GB:
HIGH NOISE:
<img width="974" height="579" alt="Screenshot 2026-01-31 141055" src="https://github.com/user-attachments/assets/e1ea9c6d-9d5f-43ef-a010-bf5328bcbf75" />

LOW NOISE:
<img width="999" height="576" alt="Screenshot 2026-01-31 141622" src="https://github.com/user-attachments/assets/e8236f42-0e98-44e3-8aad-05c805103b20" />

## GRAPH OF 10GB:
HIGH NOISE:
<img width="967" height="750" alt="Screenshot 2026-01-31 143335" src="https://github.com/user-attachments/assets/a15e79e3-8c2e-4208-8a74-d36a9a36b16a" />

LOW NOISE:
<img width="997" height="769" alt="Screenshot 2026-01-31 143456" src="https://github.com/user-attachments/assets/10a3d23f-7138-466f-95a1-dd00a5c3f26b" />


## DESCRIPTION:
Attenuation measurement at 2.5 Gbps and 10 Gbps evaluates the optical power loss in a fiber due to absorption, scattering, and connection losses. This measured attenuation determines the attenuation-limited fiber length, which is the maximum distance the signal can travel while still maintaining sufficient power at the receiver for reliable communication.

## Analysis and Report
Compare simulation results with pre-lab calculations and record observations.  

Your report should contain:
- **Cover Page**
  - Title of the lab  
  - Course name and number  
  - Your name  

- **Pre-lab Calculations**  

- **Screenshots** of layout and results (including eye diagrams)  

- **Summary Table** for each simulation:
  | Fiber Length (km) | Received Power (dBm) | Q Factor | BER |
  |-------------------|-----------------------|----------|-----|
  

- **Written Summary** of observations and explanations of differences.  
## result 
thus the experiment was succesfully completed and output is verified 




