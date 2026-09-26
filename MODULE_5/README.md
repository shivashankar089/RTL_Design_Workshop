# Final Physical Design Steps

This module documents the final physical-design stages of a Sky130 RTL-to-GDSII flow. The topics include routing, design-rule checking, power distribution, global and detailed routing, and TritonRoute reports.

## Objectives

- Understand maze routing and the Lee routing algorithm.
- Review routing constraints and design-rule checking.
- Build and inspect the power-distribution network.
- Understand global routing and detailed routing.
- Run TritonRoute and analyze its routing results.
- Collect final implementation reports and evidence.

## Workflow

### 1. SKY130_D5_SK1 - Routing and Design-Rule Checking

Routing connects the placed standard cells, clock network, power network, and I/O pins according to the technology rules. Design-rule checking is used to identify physical violations before final database generation.

#### Lab steps

1. Introduction to maze routing.
2. Study the conclusions and operation of Lee's algorithm.
3. Run and review design-rule checking (DRC).

**Results to add:** routing setup, routing screenshots, DRC command, violation count, and the final DRC report.

### 2. SKY130_D5_SK2 - Power Distribution Network

The power-distribution network supplies stable power and ground to the standard cells. It includes the core power rails, straps, rings, and connections from the power pads or ports to the cell rows.

#### Lab steps

1. Build the power-distribution network.
2. Review the steps from the power-grid setup to the completed network.
3. Study the basics of global and detailed power routing.

**Results to add:** power-grid configuration, generated files, screenshots of the rails and straps, and checks for power connectivity.

### 3. SKY130_D5_SK3 - TritonRoute Flow

TritonRoute performs detailed routing after global routing has assigned approximate routing resources. The final routing stage must connect the design while respecting the Sky130 technology rules and minimizing violations.

#### Lab steps

1. Review TritonRoute feature 1.
2. Review TritonRoute feature 2.
3. Study the TritonRoute method and routing stages.
4. Analyze the routing report.

**Results to add:** TritonRoute commands, routed-layout screenshots, wire and via counts, DRC results, and routing-report observations.

## Final Checklist

- [ ] Power-distribution network generated and checked.
- [ ] Global routing completed.
- [ ] Detailed routing completed.
- [ ] DRC report collected.
- [ ] Routing report collected.
- [ ] Final layout screenshots attached.
- [ ] Final timing and area results recorded.

## Flow Summary

`power distribution` -> `global routing` -> `detailed routing` -> `TritonRoute` -> `routing report` -> `design-rule checking` -> `final layout`

## Notes and Attachments

Add the relevant screenshots, terminal commands, reports, final layout files, and conclusions below as the lab work is completed.

## Author

- **Name     :** Nukala Shiva Shankar
- **Roll No. :** 24EG104E28
- **College  :** Anurag University