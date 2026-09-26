# Design Library Cell: ngspice Characterization and Magic Layout

This module characterizes a CMOS inverter with ngspice before moving toward its physical layout in Magic. The simulation workflow uses Sky130 PDK transistor models to examine the inverter's DC transfer characteristic and the effect of device sizing on switching behavior.

## Objectives

- Prepare and run an ngspice deck for a CMOS inverter using Sky130 model files.
- Sweep the input voltage and plot the output voltage to obtain the voltage-transfer characteristic (VTC).
- Compare two inverter design cases and observe how transistor sizing affects switching behavior.
- Identify the switching threshold, $V_m$, where the input and output voltages are equal.
- Use the VTC to assess static noise margins and changes in switching behavior.
- Continue from circuit-level characterization toward standard-cell layout in Magic.

## Execution Flow

The screenshots below are arranged by the work they document, not alphabetically by filename. The first case is simulated and plotted before the second case is run and plotted.

### 1. Open and Prepare ngspice

This screenshot records the ngspice environment used for the inverter experiments. ngspice reads the circuit deck and the referenced device models, then runs the requested analysis. Confirm that the Sky130 model paths and the simulator commands are available before running either design case.

### 2. Set Up the First Inverter Case

This image documents the SPICE setup for the first design case. The deck describes the inverter circuit and its input stimulus, loads the MOSFET models, and requests a DC input sweep. This first run provides the baseline for interpreting the transfer curve. Record the transistor dimensions and sweep range shown in the deck when comparing it with the next case.

### 3. Plot the First Case's Input and Output

This plot shows the first case's output response as the input voltage is swept. The inverter's transition region is where the output changes from its high level toward its low level. The approximate switching threshold $V_m$ can be read where $V_{in}=V_{out}$; use the plotted axes and data to determine its value rather than assuming it from the supply voltage.

### 4. Set Up the Second Inverter Case

This image documents the SPICE setup for the second design case. Compare its device dimensions and analysis settings with the first deck to identify the intended change, such as a transistor-sizing adjustment. Keeping the supply, input sweep, and model setup consistent makes the resulting VTCs easier to compare.

### 5. Plot the Second Case and Compare the Results

This plot shows the second case's input-output response. Compare its transition region and the point where $V_{in}=V_{out}$ with the first plot. A shift in the transition indicates a change in switching threshold; the steepness and shape of each curve also help assess the inverter's switching behavior. Noise margins can be evaluated from the VTC by identifying the valid logic-level boundaries and the corresponding low- and high-input limits.

## Flow Summary

`ngspice environment` -> `first inverter deck` -> `first VTC plot` -> `second inverter deck` -> `second VTC plot` -> `compare switching behavior` -> `continue to Magic layout`

## Magic Layout

The current screenshots document ngspice setup and inverter characterization. Add the Magic layout screenshots and their explanations here as that part of the work is completed. The physical-layout stage follows circuit-level characterization; its implementation details and results are not represented by the five screenshots currently included in this folder.

## Author

- **Name     :** Nukala Shiva Shankar
- **Roll No. :** 24EG104E28
- **College  :** Anurag University