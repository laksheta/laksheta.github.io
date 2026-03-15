---
title: "7kW DAB Controller Implementation"
excerpt: "Translated complex control logic from PLECS simulation to a physical 7kW DAB prototype using PLECS Coder and TI F28379D. <br/><img src='/images/portofolio/4/header.jpg' width='1000'>"
collection: portfolio
# classes: wide
---

## Project Overview
A 7 kW Dual-Active Bridge (DAB) prototype was developed to validate advanced control implementations on real power hardware. As part of the **Universitas Gadjah Mada – PT PLN (Persero) Collaboration**, this work focused on bridging simulation results with real-time experimental testing.

---

## Core Contributions & Technical Execution

### 1. Controller Code Generation & Deployment
* **The Challenge:** High-power hardware requires a reliable transition from idealized simulation to real-time executable code to ensure safety and performance.
* **My Execution:** I utilized **PLECS Coder** to generate hardware-compatible C-code directly from the control models. This workflow involved optimizing the simulation blocks for the **TI C2000 F28379D**, specifically managing ADC-to-PWM latency and ensuring the interrupt service routines (ISR) were optimized for the DAB’s high-frequency switching requirements.