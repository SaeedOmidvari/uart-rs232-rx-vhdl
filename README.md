# RS-232 / UART Receiver (RX) in VHDL

UART (RS-232 framing) receiver implemented in VHDL.
Includes a dedicated RX testbench and waveform-based verification.

## Features
- UART format: 8-N-1
- Start-bit detection, sampling of 8 data bits (LSB first), stop-bit check
- `Valid` pulse asserted when a byte is received
- Synthesizable RTL + simulation testbench

## Repository Structure
- `rtl/` – UART RX RTL implementation
- `tb/` – RX testbench
- `docs/` – simulation screenshots and notes

## Simulation
Behavioral simulation confirms correct byte reconstruction and `Valid` behavior.

## Target Platform
Designed for Zynq Arty Z7-20 FPGA projects.
