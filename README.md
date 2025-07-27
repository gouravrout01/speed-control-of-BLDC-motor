# speed-control-of-BLDC-motor
# 🔧 Speed Control of BLDC Motor Using PID Controller in Simulink

This project demonstrates the simulation of a **Brushless DC (BLDC) motor speed control system** using **PID control** and **electronic commutation logic** implemented in MATLAB Simulink. The simulation includes key elements like Gate Pulse generation, MOSFET switching, Hall-effect feedback signals, and a PMSM model.

![BLDC Simulink Model](images/bldc_model.png)

---

## 🌀 Overview

This project replicates a real-time control setup for BLDC motors using:

- PID controller for speed regulation
- Commutation logic using **AND gates**, **Mux/Demux**, and logic blocks
- Gate Pulse Generation for 3-phase inverter
- MOSFET-based inverter
- Hall-effect feedback signals
- Permanent Magnet Synchronous Machine (PMSM) block as the motor

---

## 📁 File Structure

```
📦 bldc-speed-control/
 ┣ 📄 project.slx               # Main Simulink model
 ┣ 📄 README.md                 # This file
 ┣ 📁 images/
 ┃ ┗ 📄 bldc_model.png          # Screenshot of the model
 ┗ 📄 LICENSE                   # (Optional) License info
```

---

## 🧰 Requirements

- MATLAB R2020a or later
- Simulink
- Simscape (optional for future expansion)
- Simscape Electrical
- Control System Toolbox (for PID)

---

## 🚀 How to Run

1. Open MATLAB.
2. Navigate to the project folder.
3. Run the command below in MATLAB:
   ```matlab
   open('project.slx');
   ```
4. Click **Run** to simulate.
5. Observe:
   - Rotor speed (rad/s)
   - Electromagnetic torque (N·m)
   - Gate pulses
   - Hall-effect sensor outputs

---

## ⚙️ Functional Blocks

- **PID Controller**: Maintains desired rotor speed
- **Hall-effect Sensor**: Provides position feedback for commutation
- **Commutation Logic**: Converts Hall signals into switching sequences
- **Gate Driver Logic**: Generates gate pulses for MOSFETs
- **Three-phase Inverter**: Controls power delivery to the motor
- **PMSM Block**: Represents the BLDC motor

---

## 📊 Outputs

- **Rotor Speed** vs. **Setpoint**
- **Electromagnetic Torque**
- **Commutation Switching Patterns**

---

## 📽️ Based on

This project was inspired by this helpful tutorial:  
📺 [Speed Control of BLDC Motor using PID - MATLAB/Simulink](https://youtu.be/YSkvN5FEmqc?si=tQnejUryqbK_m5d3)

---

