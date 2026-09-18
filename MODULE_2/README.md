# RTL Design Workshop - Module 2

## Floorplanning and Physical Design Using OpenLane-Style Tools

---

## Index

1. [Introduction](#1-introduction)
2. [Objective](#2-objective)
3. [ASIC Physical-Design Flow](#3-asic-physical-design-flow)
4. [Configuration and Flow Files](#4-configuration-and-flow-files)
5. [Design Statistics](#5-design-statistics)
6. [Floorplanning](#6-floorplanning)
7. [I/O Placement](#7-io-placement)
8. [Placement and Layout](#8-placement-and-layout)
9. [Floorplan Review](#9-floorplan-review)
10. [Results and Conclusion](#10-results-and-conclusion)
11. [Files](#files)
12. [Tools and Technologies](#tools-and-technologies)
13. [Key Learnings](#key-learnings)

## 1. Introduction

Module 2 covers early physical-design stages after synthesis, with emphasis on configuration, floorplanning, I/O placement, standard-cell placement, and layout visualization using SKY130-related references.

## 2. Objective

- Understand the purpose of ASIC floorplanning.
- Review core area, die area, utilization, and aspect ratio.
- Configure a physical-design flow using Tcl references.
- Study I/O placement and standard-cell placement.
- Inspect layout views and compare floorplan results.

## 3. ASIC Physical-Design Flow

The documented flow progresses through:

**RTL design -> configuration -> synthesis -> floorplanning -> I/O placement -> standard-cell placement -> layout visualization -> physical analysis**

This module focuses on how synthesized logic is organized spatially inside the die and core regions.

## 4. Configuration and Flow Files

The configuration references document the Tcl settings and commands used to run the physical-design flow. These settings control technology selection and physical implementation parameters.

## 5. Design Statistics

Design statistics help characterize the implementation before and during physical design. Useful measurements include cell and instance counts, nets, area, utilization, and overall design size.

## 6. Floorplanning

Floorplanning determines the physical dimensions and organization of the chip. Important parameters include die area, core area, aspect ratio, utilization, and available placement space. The two floorplan references provide comparison points for different physical arrangements.

## 7. I/O Placement

I/O placement determines where input and output pins are positioned around the core. Pin locations influence routing length, congestion, timing, and the quality of physical connectivity.

## 8. Placement and Layout

After floorplanning and I/O placement, standard cells are placed within the core area. The placement view provides a physical representation of the synthesized logic and supports analysis of cell distribution, wirelength, congestion, and routability.

## 9. Floorplan Review

The floorplan and layout references can be reviewed using physical-design visualization tools such as Magic. Comparing the floorplan, placement, and review images helps identify how physical constraints affect the implementation.

## 10. Results and Conclusion

The module documents the transition from physical-design configuration through floorplan generation, I/O placement, standard-cell placement, and layout review. These stages provide the foundation for later clock-tree synthesis, routing, and signoff analysis.

## Files

- [config_tcls.png](config_tcls.png) - Physical-design configuration Tcl reference.
- [design _stats.png](design%20_stats.png) - Design statistics reference.
- [floorplan_1.png](floorplan_1.png) - First floorplan view.
- [floorplan_2.png](floorplan_2.png) - Additional floorplan view.
- [floorplan_magic_layout1.png](floorplan_magic_layout1.png) - Magic floorplan layout view.
- [ioplacer.png](ioplacer.png) - I/O placement result.
- [placement_layout1.png](placement_layout1.png) - Standard-cell placement layout.
- [readme_ma.png](readme_ma.png) - Flow or tool reference image.
- [results _loorplan.png](results%20_loorplan.png) - Floorplan results.
- [review_floorplan.png](review_floorplan.png) - Floorplan review result.
- [run floor_plan.png](run%20floor_plan.png) - Floorplan run reference.
- [sky130 _review floorplan.png](sky130%20_review%20floorplan.png) - SKY130 floorplan review.

## Tools and Technologies

- Verilog / RTL
- OpenLane-style physical-design flow references
- OpenROAD-style physical-design stages
- Magic
- SKY130 PDK references
- Tcl
- Linux / Ubuntu

## Key Learnings

- ASIC floorplanning
- Core and die dimensions
- Utilization and aspect ratio
- I/O placement
- Standard-cell placement
- Layout visualization
- Physical-design review
