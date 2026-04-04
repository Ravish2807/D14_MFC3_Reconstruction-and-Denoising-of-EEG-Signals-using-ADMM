<p align="center">
  <img src="logo.svg" alt="Project Logo" width="300">
</p>

<div align="center">

# $$\huge \color{#007ACC}{\text{Mathematics for Computing 3}}$$

## $$\Large \color{#D9730D}{\mathbf{Analog\ Computing\ using\ Op-Amps\ for\ SHM}}$$

![Tech](https://img.shields.io/badge/Tools-Analog%20Circuits%20|%20ADALM2000%20|%20Scopy-blueviolet?style=for-the-badge)

</div>

<p align="center">
  Presented by: <b>Group-14, AIE-D</b>
</p>

---

### 👥 Team Members
| Name | Roll Number |
| :--- | :--- |
| <img src="https://img.shields.io/badge/Ravishanmugam%20K-blue?style=flat-square" /> | `CB.SC.U4AIE24347` |
| <img src="https://img.shields.io/badge/Sharvesh%20Sivaganam-blue?style=flat-square" /> | `CB.SC.U4AIE24355` |
| <img src="https://img.shields.io/badge/Sri%20Harini%20MP-blue?style=flat-square" /> | `CB.SC.U4AIE24358` |
| <img src="https://img.shields.io/badge/Vignes%20VM-blue?style=flat-square" /> | `CB.SC.U4AIE24359` |

---

## 📑 Table of Contents
- [Project Overview](#-project-overview)
- [Objective](#-objective)
- [Theoretical Background](#-theoretical-background)
- [Components Used](#-components-used)
- [Circuit Design](#-circuit-design)
- [Hardware Implementation](#-hardware-implementation)
- [Testing & Setup](#-testing--setup)
- [Results](#-results)
- [Conclusion](#-conclusion)
- [References](#-references)

---

> [!IMPORTANT]
> **Project Overview:** This project demonstrates solving the **Simple Harmonic Motion (SHM)** differential equation using **Analog Computing with Operational Amplifiers**.

---

## 📌 Project Overview

This project focuses on implementing **Analog Computing** to solve a **second-order Ordinary Differential Equation (ODE)** representing **Simple Harmonic Motion (SHM)**.

Unlike digital computation, this system uses **continuous electrical signals** to model and solve equations in real-time using Op-Amps and integrator circuits.

---

## 🎯 Objective

- Understand **Analog Computing principles**
- Solve **ODE using hardware circuits**
- Implement **SHM using Op-Amps**
- Use **ADALM2000 (M2K)** for real-time testing

---

## 🧠 Theoretical Background

### 🔹 SHM Equation

\[
\frac{d^2x}{dt^2} + \omega^2 x = 0
\]

This equation is implemented using:
- Integrators (to compute derivatives)
- Feedback loops (to maintain oscillation)

---

## 🔧 Components Used

- μA741 Operational Amplifiers  
- Resistors (10kΩ, 1MΩ, 1kΩ)  
- Capacitors (0.1µF)  
- Breadboard  
- Connecting wires  
- ADALM2000 (M2K)  
- Scopy Software  

---

## 🔌 Circuit Design


::contentReference[oaicite:0]{index=0}


- Uses **3 Op-Amps**
- First two → Integrators  
- Third → Feedback control  
- Closed loop generates oscillation  

---

## 🛠️ Hardware Implementation


::contentReference[oaicite:1]{index=1}


- Built using breadboard + M2K  
- Proper resistor-capacitor placement  
- Loop connections established  

---

## ⚙️ Testing & Setup


::contentReference[oaicite:2]{index=2}


### Steps:
1. Provide ±5V supply  
2. Apply initial voltages:
   - +3V (Op-Amp 1)
   - +4V (Op-Amp 2)
3. Observe waveform using oscilloscope  
4. Remove initial input after stabilization  

---

## 📊 Results


::contentReference[oaicite:3]{index=3}


- Channel 1 → Sinusoidal waveform  
- Channel 2 → Phase-shifted signal  
- Confirms SHM behavior  

---

## 🚀 Conclusion

This project successfully demonstrates that:

- Analog circuits can **solve differential equations directly**
- SHM can be modeled using **Op-Amps and integrators**
- Analog computing enables **real-time, continuous computation**

It highlights the importance of analog systems in:
- Signal processing  
- Control systems  
- Hardware-based computation  

---

## 📚 References

1. Sedra, A. S., & Smith, K. C.  
   *Microelectronic Circuits*  

2. Boylestad, R. L., & Nashelsky, L.  
   *Electronic Devices and Circuit Theory*  

3. Analog Devices Inc.  
   *ADALM2000 Active Learning Module Documentation*  

4. Oppenheim, A. V., & Schafer, R. W.  
   *Signals and Systems*  

5. Haykin, S., & Van Veen, B.  
   *Signals and Systems*  

---