# RTL Design Workshop - Day 4

This folder examines mux coding styles, blocking assignments, and the resulting RTL and synthesized views.

## Files

- [bad_mux_gtk.png](bad_mux_gtk.png) - GTKWave result for the problematic mux implementation.
- [bad_mux_yosys.png](bad_mux_yosys.png) - Yosys synthesis view of the problematic mux implementation.
- [blocking_caveat_gtk.png](blocking_caveat_gtk.png) - GTKWave example demonstrating a blocking-assignment caveat.
- [blocking_caveat_yosys.png](blocking_caveat_yosys.png) - Yosys view associated with the blocking-assignment example.
- [ternary_operator_mux_rtl.png](ternary_operator_mux_rtl.png) - RTL view of a mux written with the ternary operator.
- [ternary_operator_mux_yoys_rtl.png](ternary_operator_mux_yoys_rtl.png) - Yosys RTL view of the ternary-operator mux.

The `bad_mux` and `blocking_caveat` screenshots are comparison examples for identifying unintended simulation or synthesis behavior. The ternary-operator images show a compact alternative for describing mux logic.
