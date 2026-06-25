# Si-SiGe-Heterojunction-Line-TFET-Simulation-using-Sentaurus-TCAD


## Overview

This project presents the modeling and simulation of a Si/SiGe heterojunction Line Tunnel Field-Effect Transistor (L-TFET) using Synopsys Sentaurus TCAD.

The device geometry and doping profile were implemented using parameters reported in published literature.The objective of this project was to develop a functional TCAD model of a Si/SiGe heterojunction Line TFET and investigate its operation through transfer-characteristic simulations, energy-band analysis, and tunneling-related carrier transport.

## Device Description

The modeled device consists of:

* SiGe source region
* Silicon channel region
* Silicon drain region
* Thin epitaxial tunneling layer
* HfO₂ gate dielectric
* Single-gate Line TFET architecture

The heterojunction between SiGe and Si enhances carrier tunneling by reducing the effective tunneling barrier, enabling lower-voltage device operation compared to conventional MOSFET structures.

## Simulation Methodology

The simulation was performed using Synopsys Sentaurus TCAD.

### Workflow

1. Built a Si/SiGe heterojunction Line TFET structure using SDE.
2. Defined material properties and doping concentrations based on published literature.
3. Configured tunneling and carrier transport models.
4. Simulated the device under varying gate bias conditions.
5. Analyzed transfer characteristics, energy-band profiles, and tunneling behavior using SVISUAL.

### Physics Models

The simulation setup included:

* Fermi statistics
* Shockley–Read–Hall (SRH) recombination
* Auger recombination
* Bandgap narrowing
* Field-dependent mobility models
* Non-local tunneling models

## Results

### Device Structure

![Device Structure](results/device_structure.png)

The figure above shows the simulated Si/SiGe heterojunction Line TFET geometry used in Sentaurus TCAD.

---

### Transfer Characteristics (Id–Vg)

![Transfer Characteristics](results/transfer_curve.png)

The transfer characteristics were obtained by sweeping the gate voltage while maintaining a fixed drain bias. The results demonstrate the switching behavior of the Line TFET and the increase in drain current with increasing gate voltage.

---

### Band Diagram

![Band Diagram](results/band_diagram.png)

The energy band diagram illustrates the conduction band, valence band, and quasi-Fermi levels across the device under bias conditions. Band bending near the heterojunction region enables carrier tunneling, which forms the basis of TFET operation.

---

### Electric Field Distribution

![Electric Field Distribution](results/electric_field.png)

The electric field profile highlights regions of strong field concentration near the tunneling junction, which directly influence carrier tunneling probability and device performance.

---

### Tunneling Distribution

![Tunneling Distribution](results/tunneling_contour.png)

Spatial distributions of tunneling-related quantities were analyzed to identify active tunneling regions within the device structure.

## Key Observations

* Successful implementation of a Si/SiGe heterojunction Line TFET in Sentaurus TCAD.
* Drain current increases with gate voltage due to enhanced tunneling probability.
* Electric field concentration is strongest near the tunneling junction.
* Device operation is governed by tunneling-based carrier transport rather than conventional thermionic emission.
* Band diagrams and tunneling profiles provide insight into the underlying device physics.

## Tools Used

* Synopsys Sentaurus Structure Editor (SDE)
* Synopsys Sentaurus Device
* Synopsys Sentaurus Visual

## Reference

Device dimensions and doping parameters were adapted from published literature on Si/SiGe heterojunction Line TFETs. This repository contains an independent TCAD implementation and analysis of the device structure.
S. Panwar, S. Srivastava, M. Shashidhara and A. Acharya, "Performance Evaluation of High-κ Dielectric Ferro-Spacer Engineered Si/SiGe Hetero-Junction Line TFETs: A TCAD Approach," in IEEE Transactions on Dielectrics and Electrical Insulation, vol. 30, no. 3, pp. 1066-1071, June 2023, doi: 10.1109/TDEI.2023.3266413.
keywords: {Logic gates;Tunneling;Performance evaluation;Junctions;Semiconductor process modeling;TFETs;Epitaxial layers;Band-to-band tunneling (BTBT);ferroelectric (FE) spacer;high-κ dielectrics;line-tunnel field-effect transistor (L-TFET);remanent polarization;saturation polarization;technology computer-aided design (TCAD)},


