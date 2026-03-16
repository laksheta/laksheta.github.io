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
  <img src="/images/portofolio/5/1_1.png" alt="Rectifier Simulation" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/5/1_2.png" alt="SCADA Rectifier Result" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. MMC Rectifier: Typhoon HIL averaged-model simulation (top) and SCADA monitoring result (bottom).</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/5/1_3.jpg" alt="DAB Simulation" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/5/1_4.png" alt="SCADA DAB Result" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 2. DAB Stage: Typhoon HIL averaged-model simulation (top) and SCADA monitoring result (bottom).</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/5/1_5.jpg" alt="Inverter Simulation" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd; margin-bottom: 10px;">
  <img src="/images/portofolio/5/1_6.png" alt="SCADA Inverter Result" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 3. MMC Inverter: Typhoon HIL averaged-model simulation (top) and SCADA monitoring result (bottom).</i></p>
</div>

### 2. Integrated SST System Simulation
* **The Challenge:** Integrating the rectifier, DAB, and inverter stages into a single, unified SST system simulation.
* **My Execution:** I unified the developed averaged models into a single **Typhoon HIL** schematic. This integrated setup provides a robust platform for analyzing multi-stage interactions, DC-link energy balance, and overall system response to grid disturbances without the overhead of detailed switching models.