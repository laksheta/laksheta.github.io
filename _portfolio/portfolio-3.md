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
* **My Execution:** I designed and validated the following algorithms in **PLECS**:
    * **MMC Rectifier:** Designed the algorithm to precharge sub-module capacitors [1] in collaboration with teammate Ariq Naufal Fakri Wiratno.
    * **DAB Startup:** Developed a soft-start algorithm by ramping up the phase shift [2] to ensure stable power transfer.
    * **MMC Inverter:** Designed the algorithm to precharge sub-module capacitors [1] for stable grid/load integration.

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/3/1_1.png" alt="MMC Rectifier" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 1. MMC rectifier with startup algorithm.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/3/1_2.png" alt="DAB" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 2. DAB with startup algorithm.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/3/1_3.png" alt="MMC Inverter" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 3. MMC inverter with startup algorithm.</i></p>
</div>
---

### 2. SST System Coordination
* **The Challenge:** The integrated SST requires configuration scenarios to ensure the MMC rectifier, DAB, and MMC inverter stages interface and synchronize correctly during operation.
* **My Execution:** I designed **the master coordination framework** for the SST system by developing logic-driven operational scenarios in **PLECS**. 

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/3/2_1.jpg" alt="Master Control" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 4. Master control implementation for the integrated SST system.</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/3/2_2.jpg" alt="MMC Rectifier Result" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 5. MMC rectifier stage result (integrated SST simulation).</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/3/2_3.jpg" alt="DAB Result" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 6. DAB stage result (integrated SST simulation).</i></p>
</div>

<div style="text-align: center; margin: 25px 0;">
  <img src="/images/portofolio/3/2_4.jpg" alt="MMC Inverter Result" style="max-width: 80%; border-radius: 6px; border: 1px solid #ddd;">
  <p style="font-size: 0.9em; color: #555;"><i>Figure 7. MMC inverter stage result (integrated SST simulation).</i></p>
</div>

## References
[1] L. Zhang, J. Qin, X. Wu, S. Debnath and M. Saeedifard, "A Generalized Precharging Strategy for Soft Startup Process of the Modular Multilevel Converter-Based HVDC Systems," in IEEE Transactions on Industry Applications, vol. 53, no. 6, pp. 5645-5657, Nov.-Dec. 2017, doi: 10.1109/TIA.2017.2736958.

[2] F. Giuliani, N. Delmonte, P. Cova, A. Costabeber and A. Castellazzi, "Soft-starting procedure for dual active bridge converter," 2015 IEEE 16th Workshop on Control and Modeling for Power Electronics (COMPEL), Vancouver, BC, Canada, 2015, pp. 1-6, doi: 10.1109/COMPEL.2015.7236516.