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
