# 🏍️ Smart Electronic Hazard Light System – TVS Raider

A soft-touch electronic hazard light system designed and integrated into a TVS Raider motorcycle using an NE555 timer in bi-stable mode. The system replaces a mechanical toggle switch with a stable, noise-hardened electronic latch suitable for automotive environments.

---

## 📌 Project Overview

This project demonstrates the complete engineering lifecycle:

- Circuit design & simulation
- Breadboard prototyping
- Automotive noise hardening
- Final vehicle integration

The hazard system toggles ON/OFF with a push button and uses the bike’s original flasher unit for blinking.

---

## 🎯 Objectives

- Replace bulky mechanical toggle with electronic latch
- Ensure stable operation in noisy motorcycle environment
- Prevent false triggering due to EMI
- Integrate cleanly with stock wiring
- Maintain OEM-style flashing behavior

---

## 🧠 System Architecture

### Core Components

- NE555 Timer (Bi-stable mode)
- S8050 NPN Transistor
- 12V Relay
- LM7805 Voltage Regulator
- RC Network (100kΩ + 1µF)
- Flyback Diode
- Noise Filtering Capacitors

---

## ⚙️ Working Principle

### 1️⃣ Latching Mechanism (NE555)

- Configured in bi-stable mode  
- Push button toggles output state  
- RC network ensures stable switching  

### 2️⃣ Relay Driving Stage

- S8050 used as switching transistor  
- Relay coil driven via transistor  
- Flyback diode protects against back EMF  

### 3️⃣ Noise Hardening

- LM7805 provides regulated 5V  
- 10nF capacitor on Pin 5 filters EMI  
- Proper grounding prevents false triggering  

### 4️⃣ Hazard Logic

- Relay bridges left and right indicator lines  
- Original flasher unit controls blinking  
- Ensures factory-level timing behavior  

---

## 🔬 Engineering Challenges Solved

- Transistor pinout troubleshooting (Emitter-Base-Collector)
- Push-button bounce (double-click issue)
- Voltage spikes (12V–14.5V fluctuation)
- Ignition coil EMI interference
- Automotive power instability

---

---

## 🛠 Technical Highlights

### Transistor Saturation Design

Relay current requirement calculated to ensure:

Base Current ≥ Collector Current / β

Overdriven base guarantees full saturation and reliable switching.

---

### Power Stability

- Input voltage: 12V–14.5V
- Regulated logic voltage: 5V
- EMI filtering implemented
- Relay isolation protects logic IC

---

## 📸 Demonstrations Included

- Workbench testing video  
- Final on-bike testing video  
- Complete circuit image  
- Simulation configuration file  

---

## 📈 Skills Demonstrated

- Analog electronics design  
- Automotive electrical integration  
- Noise mitigation techniques  
- Hardware debugging  
- System-level engineering thinking  
- Simulation to real-world transition  

---

## 🚀 Future Improvements

- Replace relay with MOSFET switching
- Design custom PCB
- Add waterproof enclosure
- Add microcontroller-based programmable features

---

## 🏁 Conclusion

This project evolved from a simulated soft-touch toggle concept into a fully integrated, noise-hardened automotive solution. It demonstrates practical embedded system engineering, real-world debugging, and robust system integration.

---

**Author:** Mohammed Fawaz Ali  
B.Tech – Computer Science Engineering  
SR University, Warangal
