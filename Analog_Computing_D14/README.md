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
- [Drive Files](#-drive-files)
- [Conclusion](#-conclusion)
- [References](#-references)

---

> [!IMPORTANT]
> **Project Overview:** This project demonstrates solving the **Simple Harmonic Motion (SHM)** differential equation using **Analog Computing with Operational Amplifiers**.

---

## 📌 Project Overview

This project focuses on implementing **Analog Computing** to solve a **second-order Ordinary Differential Equation (ODE)** representing **Simple Harmonic Motion (SHM)**.

Unlike digital systems, this approach uses **continuous electrical signals** and Op-Amp circuits to compute results in real time.

---

## 🎯 Objective

- Understand **Analog Computing principles**
- Solve **ODE using hardware circuits**
- Implement **SHM using Op-Amps**
- Use **ADALM2000 (M2K)** for real-time testing

---

## 🧠 Theoretical Background

### 🔹 SHM Equation

`d²x/dt² + ω²x = 0`

Where:
- x → displacement  
- ω → angular frequency  

---

### 🔹 Conversion to First-Order System

`dx/dt = v`  
`dv/dt = -ω²x`

---

### 🔹 Inverting Amplifier

`Av = -Rf / Rin`  
`Vout = -(Rf / Rin) × Vin`

---

### 🔹 Integrator Circuit

`Vout = -(1/RC) ∫ Vin dt`

---

### 🔹 Oscillation Condition

`ω = 1 / √(RC)`

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

![Circuit Setup](image1.png)

---

## 🛠️ Hardware Implementation

![Components Used](image2.png)  
![Hardware Assembly](image3.png)

---

## ⚙️ Testing & Setup

![Testing Setup](image4.png)  
![Initial Setup](image5.png)

---

## 📊 Results

![Result Waveform](image6.png)

- Channel 1 → Sinusoidal waveform  
- Channel 2 → Phase-shifted waveform  
- Confirms SHM behavior  

---

## 🔗 Drive Files

📂 **Analog Computing Testing Files:**  
👉 https://drive.google.com/file/d/1TJnMbFOhWlprs_c0pAqsaYrTg5DkpIr1/view?usp=sharing  

---

## 🚀 Conclusion

This project demonstrates that:

- Analog circuits can **solve differential equations directly**
- SHM can be implemented using **Op-Amps and integrators**
- Analog computing enables **real-time continuous computation**

This highlights its importance in:
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
