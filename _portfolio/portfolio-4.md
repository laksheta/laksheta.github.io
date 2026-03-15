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
* **My Execution:** I utilized **PLECS Coder** to generate hardware-compatible C code from the control models for the **TI Launchpad F28379D**.

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/4/1.png" alt="PLECS Implementation" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. Controller logic implementation in the PLECS environment.</i></p>
</div>

### 2. Startup to Closed-Loop Performance Validation
* **The Challenge:** Validating the developed control algorithm on a physical 7kW DAB prototype to ensure stability and safety under high-power conditions.
* **My Execution:** I used **PLECS Coder** to generate real-time C code from the developed control logic for the **TI Launchpad F28379D**. I then validated the system experimentally on the 7 kW DAB prototype, confirming stable startup and reliable closed-loop regulation.