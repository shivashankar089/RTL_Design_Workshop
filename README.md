# RTL Design Workshop

This repository documents an RTL design workshop that progresses from basic combinational and sequential logic to synthesis, timing analysis, and physical-design preparation. Each folder contains the related design references, simulation waveforms, RTL views, synthesis results, or implementation screenshots.

## Workshop Contents

### Days

- [Day 1](DAY_1/README.md) - Multiplexer RTL and visual verification using GTKWave references.
- [Day 2](DAY_2/README.md) - Flip-flops, asynchronous and synchronous reset behavior, module hierarchy, and synthesized netlists.
- [Day 3](DAY_3/README.md) - Constant-driven logic, counters, synthesis optimization, and RTL-versus-synthesized views.
- [Day 4](DAY_4/README.md) - Mux coding styles, ternary operators, blocking-assignment caveats, and synthesis comparisons.
- [Day 5](DAY_5/README.md) - `case` and `if` coding, incomplete assignments, generated muxes and demuxes, and a ripple-carry adder.
- [Day 6](DAY_6/README.md) - Pre-synthesis and post-synthesis design comparisons.
- [Day 7](DAY_7/README.md) - Sequence-detector simulation, output behavior, RTL waveforms, and synthesized schematic views.

### Modules

- [Module 1](MODULE_1/README.md) - PicoRV32A RTL-to-synthesis flow, Tcl configuration, design inspection, synthesis statistics, SKY130 setup, netlist generation, and OpenSTA timing reports.
- [Module 2](MODULE_2/README.md) - Physical-design preparation, including configuration, design statistics, floorplanning, IO placement, standard-cell placement, Magic layout views, and floorplan review.

## Learning Progression

1. Describe combinational logic and sequential elements in RTL.
2. Understand reset behavior, hierarchy, and the effects of coding style.
3. Identify incomplete assignments and common simulation or synthesis issues.
4. Compare RTL, synthesized netlists, waveforms, and schematics.
5. Run synthesis and review implementation statistics and timing.
6. Continue from synthesis into floorplanning, placement, and layout inspection.
