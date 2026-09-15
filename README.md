# FPGA Mini Projects

A collection of 17 small digital-design exercises built in Xilinx Vivado while learning Verilog HDL and FPGA workflows during an internship at NIELIT Calicut (May–July 2025). Each sub-folder under `projects/` is a separate Vivado project targeting Xilinx 7-series parts, ranging from basic combinational logic to small FSM-based applications.

## Repository contents

This repo currently contains the **Vivado project files (`.xpr`) only** — no Verilog source, testbenches, or `.xdc` constraint files are committed. Opening a `.xpr` in Vivado will not build correctly on its own; the underlying source lives on the original development machine and has not been added to version control yet. What you can verify from this repo:

- 17 `.xpr` project shells in `projects/`, one per mini-project
- A handful of hardware demo videos in `demos/videos/`
- One photo of a Basys-3 board in `images/`

## Projects

| Project | File | Description |
|---|---|---|
| 4-Bit Adder | `4bitadder.xpr` | 4-bit binary adder |
| Ripple Carry Adder | `RCA.xpr` | Multi-bit adder built from cascaded full adders |
| FPGA ALU | `fpgaALU.xpr` | Small ALU with arithmetic operations, driven to a 7-segment display |
| Magnitude Comparator | `mag_comp.xpr` | Compares two binary values (>, <, =) |
| BCD to 7-Segment | `BCD7seg.xpr` | Converts a BCD input to 7-segment display patterns |
| PWM LED Control | `pwmLed.xpr` | PWM-based LED brightness control |
| 4x1 Multiplexer | `mux4x1.xpr` | 4-to-1 data selector |
| Bitwise Operations | `bitwiseops.xpr` | AND / OR / XOR / NOT logic exercise |
| Flip-Flops | `flipflops.xpr` | D, T, JK, and SR flip-flop implementations |
| Sequential Circuit | `sqlckt.xpr` | Sequential logic / state machine exercise |
| Stop-Wait-Go | `stopwaitgo.xpr` | Traffic-light style FSM controller |
| FIR Filter | `FIRfilter.xpr` | Small FIR filter exercise |
| EPC | `EPC.xpr` | Encoder/parity-check style exercise |
| Digital Safe System | `digsafesystem.xpr` | Code-entry based access/security exercise |
| Car Parking System | `carpark.xpr` | Parking-slot counter/controller |
| Test IP | `testIP.xpr` | Scratch project for testing a Vivado IP core |
| Parallel Practice | `parapractice.xpr` | General combinational/sequential practice exercise |

Descriptions above are inferred from project names and the project metadata; since no HDL source is included, exact functionality can't be independently verified from this repo alone.

## Tools and hardware

- **Toolchain:** Xilinx Vivado 2024.1
- **Target parts:** Most projects are configured for the Basys-3 board's Artix-7 part (`xc7a35tcpg236-1`) or the Arty A7's part (`xc7a35tcsg324-1`); several project files still carry Vivado's default part (`xc7k70tfbv676-1`, a Kintex-7) and were not tied to a specific board
- **Confirmed hardware:** the photo in `images/basys3_demo.jpeg` and the videos in `demos/videos/` show a Digilent Basys-3 board running the 7-segment/counter examples

## Demo videos

- `demos/videos/alu_demo_1.mp4`, `alu_demo_2.mp4` — ALU running on hardware
- `demos/videos/seven_segment_demo.mp4` — 7-segment display multiplexing
- `demos/videos/led_counter_demo.mp4` — LED counter demo

## Opening a project

```bash
git clone https://github.com/DarkDragoXE/FPGA-Based-Mini-projects.git
```

In Vivado: `File → Open Project → projects/<name>.xpr`. Note that since source files aren't included, most projects will need HDL/constraint files re-added before they synthesize.

## Author

Debtonu Bose ([DarkDragoXE](https://github.com/DarkDragoXE))
