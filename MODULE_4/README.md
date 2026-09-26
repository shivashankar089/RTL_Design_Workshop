# Pre-Layout Timing Analysis and Clock Design

This module documents pre-layout timing analysis for a Sky130 design. It introduces timing models, standard-cell delay information, setup and hold analysis, clock-tree synthesis, and the importance of a well-designed clock network before detailed routing.

## Objectives

- Understand how timing information is modeled before physical design.
- Convert placement-grid information into routing-track information.
- Use standard-cell delay tables to understand propagation delay.
- Perform setup and hold timing analysis.
- Understand clock-tree routing, clock skew, and clock crosstalk.
- Run and verify clock-tree synthesis (CTS).

## Workflow

### 1. SKY130_D4_SK1 - Timing Modeling

This section introduces the timing model used by the Sky130 standard-cell library. Record the design, library, clock, and timing-model files used in the lab here.

#### Lab steps

1. Convert grid information to track information.
2. Review the relationship between placement grids and routing tracks.
3. Study the introduction to timing and timing terminology.
4. Study the introduction to cell and path delay.
5. Use delay tables - Part 1.
6. Use delay tables - Part 2.
7. Configure the timing-analysis environment.

**Evidence to add:** screenshots, commands, timing-model files, and observations.

### 2. SKY130_D4_SK2 - Timing Analysis

This section covers static timing analysis using the pre-layout design and its clock constraints. Setup analysis checks whether data arrives before the active clock edge, while hold analysis checks whether data remains stable for the required time after the edge.

#### Lab steps

1. Set up the timing-analysis environment.
2. Introduce clock timing and clock constraints.
3. Configure the timing-analysis inputs.
4. Optimize the design for timing.
5. Perform a basic timing analysis and record the critical paths.

**Results to add:** clock period, setup slack, hold slack, worst paths, and screenshots of the reports.

### 3. SKY130_D4_SK3 - Clock Tree Synthesis

Clock-tree synthesis distributes the clock from its source to sequential elements while controlling skew, latency, transition time, and load. A balanced clock tree helps the design meet setup and hold requirements.

#### Lab steps

1. Review clock-tree routing and clock distribution.
2. Study crosstalk and clock-noise effects.
3. Run clock-tree synthesis.
4. Verify the CTS results and timing reports.

**Results to add:** CTS command, clock-tree report, skew, latency, buffer count, and before/after timing results.

### 4. SKY130_D4_SK4 - Timing Analysis After CTS

This section analyzes timing after clock-tree synthesis. The propagated clock is now used to evaluate the effect of real clock latency and skew on setup and hold timing.

#### Lab steps

1. Set up post-CTS timing analysis.
2. Perform hold-timing analysis using real clocks.
3. Analyze timing violations and identify the affected paths.
4. Apply timing fixes and extend the analysis as required.
5. Observe and record the final timing results.

**Results to add:** post-CTS setup and hold reports, violation count, slack values, and screenshots.

## Flow Summary

`timing model` -> `grid and track information` -> `delay tables` -> `setup analysis` -> `hold analysis` -> `clock-tree synthesis` -> `post-CTS timing verification`

## Notes and Attachments

Add the relevant screenshots, terminal commands, report files, waveforms, and conclusions below as the lab work is completed.

## Author

- **Name     :** Nukala Shiva Shankar
- **Roll No. :** 24EG104E28
- **College  :** Anurag University