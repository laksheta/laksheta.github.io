---
title: "Multi-DSP Control Implementation for MMC"
excerpt: "Programmed Modular Multilevel Converters (MMC) control logic for multi-DSP systems (F28379D, F280049C) and validated full-scale SST performance using Typhoon HIL 604. <br/><img src='/images/portofolio/2/header.jpg' width='300'>"
collection: portfolio
# classes: wide
---

## Project Overview
This project, part of the **Universitas Gadjah Mada – PT PLN (Persero) Collaboration**, focused on the real-time validation of Modular Multilevel Converters (MMC) within a Solid-State Transformer (SST) architecture to ensure system stability and regulation under industrial conditions.

---

## Core Contributions & Technical Execution

### 1. Multi-DSP Embedded Control Development
* **The Challenge:** Integration and real-time validation of the MMC control logic, developed by teammate Lathief Nurmahmudi, onto the TI C2000 hardware platform.
* **My Execution:** I utilized **PLECS Coder** to generate and deploy control code across **TI C2000 microcontrollers (F280049C, F28069M, and F28379D)** and engineered the signal routing and timing synchronization between the multiple DSPs.

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/1_1.png" alt="Configuration" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. Multi-DSP hardware architecture diagram for MMC control.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/1_2.jpg" alt="Cable connection" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 2. Physical wiring setup showing signal routing between multiple TI C2000 Launchpads.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/1_3.png" alt="Master side" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 3. PLECS control logic implementation for the Master-side controller.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/1_4.png" alt="Slave Phase A Control" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/2/1_5.png" alt="Slave Phase A PWM and CAN" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 4. PLECS simulation for Slave-side Phase A controller.</i></p>
</div>

---

### 2. HIL System Integration Support
* **The Challenge:** Real-time hardware-in-the-loop validation of the MMC stages within a SST architecture. This process requires precise synchronization between the HIL simulation and the multi-DSP hardware.
* **My Execution:** While my teammate, Musyaffa’ Ahmad, operated the **Typhoon HIL 604**, I managed the physical hardware interfacing for the controller side. I synchronized the **TI C2000 microcontrollers (F280049C, F28069M, and F28379D)** and troubleshot the analog/digital signal routing to ensure high-fidelity data exchange between the DSPs and the HIL I/O interface.

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/2_1.jpg" alt="Experiment setup" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/2/2_2.jpg" alt="Experiment setup" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. Multi-DSP setup for validation with Typhoon HIL</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/2_3.jpg" alt="Slave Phase A Control" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/2/2_4.jpeg" alt="Slave Phase A PWM and CAN" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 2. Validation result from Typhoon HIL.</i></p>
</div>