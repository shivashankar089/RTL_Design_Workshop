# RTL Design Workshop - Day 5

This folder focuses on conditional RTL: `case` statements, incomplete assignments, generated muxes and demuxes, and an RCA design.

## Files

- [bad_case_gls.png](bad_case_gls.png) - Gate-level simulation view of an unsafe or incomplete `case` implementation.
- [bad_case_gtk.png](bad_case_gtk.png) - GTKWave result for the bad `case` example.
- [bad_case_yosys.png](bad_case_yosys.png) - Yosys synthesis view for the bad `case` example.
- [comp_case_yosys.png](comp_case_yosys.png) - Yosys view of a complete `case` implementation.
- [demux_case_gtk.png](demux_case_gtk.png) - GTKWave view of a demultiplexer described with `case`.
- [demux_generate_gtk.png](demux_generate_gtk.png) - GTKWave view of a generated demultiplexer.
- [incomp_case_gtk.png](incomp_case_gtk.png) - GTKWave result for an incomplete `case` example.
- [incomp_case_yosys.png](incomp_case_yosys.png) - Yosys synthesis view for the incomplete `case` example.
- [incomp_if.v_gtk.png](incomp_if.v_gtk.png) - GTKWave result for an incomplete `if` assignment.
- [incomp_if2_gtk.png](incomp_if2_gtk.png) - GTKWave result for a second incomplete `if` example.
- [incomp_if2_yosys.png](incomp_if2_yosys.png) - Yosys view for the second incomplete `if` example.
- [incomp_if_yosys.png](incomp_if_yosys.png) - Yosys view for the incomplete `if` example.
- [mux_generate_gtk.png](mux_generate_gtk.png) - GTKWave view of a mux built with generate constructs.
- [mux_generate_yosys.png](mux_generate_yosys.png) - Yosys synthesis view of the generated mux.
- [partial_case_assign_yosys.png](partial_case_assign_yosys.png) - Yosys view showing the effect of partial assignments in a `case` statement.
- [rca.v_gtk.png](rca.v_gtk.png) - GTKWave view of the ripple-carry adder (`RCA`) design.

The `case` and `if` examples illustrate why every combinational output should receive a defined assignment. The generated mux and demux examples show structural repetition, and the RCA waveform provides a reference for multi-stage arithmetic logic.
