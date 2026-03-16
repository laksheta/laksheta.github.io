---
title: "Real-Time SST Simulation: Averaged-Model Optimization"
excerpt: "Developing resource-optimized SST simulations in Typhoon HIL using switching-cycle averaged models. <br/><img src='/images/portofolio/5/hil_sim_thumb.png' width='100' align='right'>"
collection: portfolio
# classes: wide
---

## Project Overview
This research focuses on developing a system-level simulation of a three-stage Solid-State Transformer (SST). The objective is to simplify computationally heavy PWM models by using an **averaged-model framework** in **Typhoon HIL**. This approach enables high-fidelity real-time analysis of the integrated **MMC rectifier, DAB, and MMC inverter** stages.

---

## Core Contributions & Technical Execution

### 1. Averaged Modeling for Individual Converters
* **The Challenge:** Detailed PWM models of Modular Multilevel Converters (MMC) and DAB stages are too computationally intensive for real-time HIL execution, often exceeding the FPGA's processing capacity.
* **My Execution:** I developed **switching-cycle averaged models** for the Rectifier, DAB, and Inverter stages in **Typhoon HIL**. Instead of modeling individual switches, the converters were represented as controlled voltage and current sources. This approach focuses the simulation on low-frequency dynamics and power flow while keeping the computation within the limits of the HIL hardware.

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/5/1_1.png" alt="Slave Phase A Control" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/5/1_2.png" alt="Slave Phase A PWM and CAN" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 4. PLECS simulation for Slave-side Phase A controller.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/5/1_3.jpg" alt="Slave Phase A Control" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/5/1_4.png" alt="Slave Phase A PWM and CAN" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 4. PLECS simulation for Slave-side Phase A controller.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/5/1_5.jpg" alt="Slave Phase A Control" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/5/1_6.png" alt="Slave Phase A PWM and CAN" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 4. PLECS simulation for Slave-side Phase A controller.</i></p>
</div>