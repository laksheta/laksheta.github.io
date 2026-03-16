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
* **My Execution:** I developed **switching-cycle averaged models** for the Rectifier, DAB, and Inverter stages within **Typhoon HIL**. By representing the converters as controlled voltage and current sources rather than individual switches, I optimized the simulation to focus on low-frequency dynamics and power flow. This approach ensures high-fidelity results at the system level while staying well within the computational limits of the HIL hardware.