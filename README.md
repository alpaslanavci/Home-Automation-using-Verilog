# EE241 Home Automation Project

## Description
This project implements a smart home system in Verilog HDL.

Project members:
- Alpaslan Avcı (20220701013)
- Adnan Tolga Aksoy (20220701011)

## Subsystems
- General management
- Lighting control (luminosity + color)
- Door control (password + lock/alarm behavior)
- Climate control (AC mode + temperature selection)
- Safety system (fire alarm + extinguisher trigger)

## Source Layout
- `AC_control.v`: AC-related modules (`temp_sel`, `AC_mode_selection`, `AC_control`)
- `door_control.v`: door control and helper modules (`t_ff`, `freq_divider`, `counter`)
- `fire.v`: fire detection state machine
- `light_control.v`: light color and luminosity control
- `top.v`: integration module (`top_module`)

Testbenches:
- `AC_control_tb.v`
- `door_control_tb.v`
- `fire_tb.v`
- `ligt_control_tb.v`
- `top_tb.v`

## Vivado Simulation Flow (Windows)
1. Open Vivado and create a new RTL project.
2. Add source files:
   - `AC_control.v`
   - `door_control.v`
   - `fire.v`
   - `light_control.v`
   - `top.v`
3. Add one testbench as simulation source:
   - `AC_control_tb.v` or `door_control_tb.v` or `fire_tb.v` or `ligt_control_tb.v` or `top_tb.v`
4. Set the selected testbench as the simulation top.
5. Run Behavioral Simulation.

Notes:
- `reset` is active-low in this design.
- `top_module` is in `top.v`.
