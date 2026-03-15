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
  <img src="/images/portofolio/2/1_1.png" alt="MMC Logic" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. PLECS control logic for multi-module MMC synchronization.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/1_2.jpg" alt="MMC Logic" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. PLECS control logic for multi-module MMC synchronization.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/1_3.png" alt="MMC Logic" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. PLECS control logic for multi-module MMC synchronization.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/1_4.png" alt="MMC Logic" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. PLECS control logic for multi-module MMC synchronization.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/1_5.png" alt="MMC Logic" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. PLECS control logic for multi-module MMC synchronization.</i></p>
</div>

---

### 2. Full-Scale SST Real-Time Validation
* **The Challenge:** High-fidelity verification of Solid-State Transformer (SST) performance under real-time constraints to match industrial standards.
* **My Execution:** I validated the SST real-time performance through high-fidelity testing on the **Typhoon HIL 604**. This involved interfacing the multi-DSP control hardware with the HIL simulator to verify the coordination between the MMC stages and the overall system response.

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/2/hil_test.jpg" alt="HIL Testing" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 2. Real-time SST performance validation using Typhoon HIL 604.</i></p>
</div>