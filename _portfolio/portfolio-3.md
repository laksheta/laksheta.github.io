---
title: "SST System-Level Integration & Coordination Design"
excerpt: "Designed sequential startup and coordination schemes for a multi-stage Solid-State Transformer (MMC-DAB-MMC) architecture using PLECS. <br/><img src='/images/portofolio/3/header.png' width='1000'>"
collection: portfolio
# classes: wide
---

## Project Overview
As part of the **Universitas Gadjah Mada – PT PLN (Persero) Collaboration**, this project focused on the high-level integration of a Solid-State Transformer (SST). The work involved designing the startup procedures and coordination logic for the three conversion stages: the **MMC rectifier**, the **Dual-Active Bridge (DAB)**, and the **MMC inverter**.

---

## Core Contributions & Technical Execution

### 1. Multi-Stage Startup Design
* **The Challenge:** Startup algorithms were required to prevent inrush currents for each individual converter and ensure a stable transition to full-system operation.
* **My Execution:** I designed and implemented the individual startup logic in **PLECS** for:
    * **MMC Rectifier:** Focused on the pre-charging phase and initial DC-link stabilization.
    * **DAB Stage:** Implemented soft-start routines to manage power transfer across the isolation barrier.
    * **MMC Inverter:** Developed the synchronization and ramp-up logic for grid or load connection.

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/3/1_2.png" alt="Startup Sequence Results" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. PLECS simulation results validating the sequential startup of the MMC and DAB stages.</i></p>
</div>

---