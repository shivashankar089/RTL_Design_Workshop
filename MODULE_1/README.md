# RTL Design Workshop - Module 1

## PicoRV32A ASIC Design Flow Using OpenLane-Style Tools

---

## Index

1. [Introduction](#1-introduction)
2. [Objective](#2-objective)
3. [Design Used](#3-design-used)
4. [ASIC Design Flow](#4-asic-design-flow)
5. [Configuration and Flow Files](#5-configuration-and-flow-files)
6. [Synthesis and Statistics](#6-synthesis-and-statistics)
7. [Netlist and Design Inspection](#7-netlist-and-design-inspection)
8. [Timing Analysis](#8-timing-analysis)
9. [Results and Conclusion](#9-results-and-conclusion)
10. [Files](#files)
11. [Tools and Technologies](#tools-and-technologies)
12. [Key Learnings](#key-learnings)

## 1. Introduction

Module 1 introduces an ASIC design flow using the PicoRV32A RISC-V processor design, the SKY130 technology references, synthesis, netlist inspection, and OpenSTA timing analysis.

## 2. Objective

- Understand the major stages of an RTL-to-ASIC flow.
- Configure a processor design and technology using Tcl references.
- Generate and inspect synthesis results.
- Review design statistics and the synthesized netlist.
- Understand the purpose of timing analysis with OpenSTA.

## 3. Design Used

PicoRV32A is a compact 32-bit RISC-V processor core used as the example design. Its size and practical structure make it useful for studying synthesis and early ASIC implementation concepts.

## 4. ASIC Design Flow

The documented flow progresses through:

**RTL design -> configuration -> synthesis -> netlist generation -> design inspection -> timing analysis -> reports**

The module emphasizes how RTL is converted into a gate-level implementation and how reports are used to understand the resulting design.

## 5. Configuration and Flow Files

Tcl configuration and flow references define design settings, technology information, and commands used by the implementation tools. The SKY130 reference connects the design flow to the target standard-cell technology.

## 6. Synthesis and Statistics

Synthesis converts the PicoRV32A RTL into a gate-level netlist. The statistics references support analysis of the synthesized design, including its structural size and implementation characteristics.

## 7. Netlist and Design Inspection

The netlist and design references provide views of the converted design. The merged-design references document intermediate flow outputs and help connect configuration commands with the generated implementation.

## 8. Timing Analysis

OpenSTA is used to inspect static timing information. Timing reports typically include paths, delays, arrival and required times, and slack. These values help determine whether the design meets its timing constraints.

## 9. Results and Conclusion

The module documents a practical synthesis and analysis flow for PicoRV32A using SKY130-related configuration references. The reports, statistics, netlist, merged-design views, and OpenSTA result provide a foundation for continuing into physical design.

## Files

- [config_tcl.png](config_tcl.png) - Configuration Tcl reference.
- [designs_picorv32a.png](designs_picorv32a.png) - PicoRV32A design setup reference.
- [flow_tcl .png](flow_tcl%20.png) - Flow Tcl reference.
- [less_cmd_tcl.png](less_cmd_tcl.png) - Command output reference.
- [less_config_tcl.png](less_config_tcl.png) - Configuration output reference.
- [less_merged 3.png](less_merged%203.png) - Merged-design output reference.
- [less_merged.png](less_merged.png) - Merged-design output reference.
- [less_merged2.png](less_merged2.png) - Additional merged-design output reference.
- [picorv32_stats1_res.png](picorv32_stats1_res.png) - PicoRV32A statistics result.
- [picorv32a _stats_res .png](picorv32a%20_stats_res%20.png) - Additional statistics result.
- [picorv32a_stats2_res.png](picorv32a_stats2_res.png) - Second statistics result.
- [picorva_dates_design.png](picorva_dates_design.png) - PicoRV32A design details.
- [report_opensta.png](report_opensta.png) - OpenSTA timing report.
- [sky130.tcl.png](sky130.tcl.png) - SKY130 technology Tcl reference.
- [syntesis_report.png](syntesis_report.png) - Synthesis report.
- [synthesis_netlist.png](synthesis_netlist.png) - Synthesized netlist view.

## Tools and Technologies

- Verilog / RTL
- PicoRV32A
- Yosys
- OpenLane-style flow references
- OpenSTA
- SKY130 PDK references
- Tcl
- Linux / Ubuntu

## Key Learnings

- RTL-to-gate-level synthesis
- RISC-V processor design inspection
- Synthesis statistics
- Netlist generation
- SKY130 technology configuration
- Static timing analysis
