---
title: "DAB Converter Control Logic & Real-Time HIL Validation"
excerpt: "Programmed and validated Dual-Active Bridge (DAB) control systems using PLECS Coder and Typhoon HIL 604. <br/><img src='/images/portofolio/1/header.jpg' width='400'>"
collection: portfolio
# classes: wide
---

## Project Overview
This project was part of a joint research collaboration between **Universitas Gadjah Mada and PT PLN (Persero)** to validate control strategies for a modular Dual-Active Bridge (DAB) system. 

## Core Contributions & Technical Execution

### 1. Embedded Implementation on TI F28069M

* **The Challenge:** My colleague, Lathief Nurmahmudi, developed the core control algorithm in simulation, which needed to be accurately translated into a real-time hardware environment for modular operation.
* **My Execution:** I utilized **PLECS Coder** to generate and deploy the control logic directly onto the **Texas Instruments F28069M Launchpad**. To facilitate the modular DAB implementation, I integrated the CAN bus protocol to establish communication between the master and slave microcontrollers.

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/1/1_1.png" alt="Master Side Implementation" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. PLECS simulation for Master-side controller.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/1/1_2.png" alt="Slave Side Implementation" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 2. PLECS simulation for Slave-side controller.</i></p>
</div>