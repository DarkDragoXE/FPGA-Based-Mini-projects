<div align="center">

# FPGA Mini Projects Collection

[![Verilog](https://img.shields.io/badge/Language-Verilog-blue.svg)](/)
[![FPGA](https://img.shields.io/badge/FPGA-Xilinx%20Artix--7-red.svg)](https://www.xilinx.com/products/silicon-devices/fpga/artix-7.html)
[![Vivado](https://img.shields.io/badge/Tool-Vivado%202024.1-orange.svg)](https://www.xilinx.com/products/design-tools/vivado.html)
[![Board](https://img.shields.io/badge/Board-Basys--3-green.svg)](https://digilent.com/shop/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)
[![Projects](https://img.shields.io/badge/Projects-17-purple.svg)](/)

**A collection of 17 digital design mini-projects implemented in Verilog HDL for the Basys-3 FPGA board**

[Projects](#projects) | [Hardware](#hardware-setup) | [Demos](#demonstrations) | [Getting Started](#getting-started)

</div>

---

## Overview

This repository contains a comprehensive collection of FPGA mini-projects designed for learning and practicing digital design concepts. Each project demonstrates fundamental to intermediate digital logic concepts, from basic combinational circuits to sequential state machines.

<div align="center">
<img src="images/basys3_demo.jpeg" alt="Basys-3 FPGA Demo" width="500"/>

*Basys-3 FPGA board running 7-segment display project*
</div>

---

## Projects

### Arithmetic Units

| Project | File | Description |
|---------|------|-------------|
| **4-Bit Adder** | `4bitadder.xpr` | Basic 4-bit binary addition circuit |
| **Ripple Carry Adder** | `RCA.xpr` | Multi-bit adder using cascaded full adders |
| **FPGA ALU** | `fpgaALU.xpr` | Arithmetic Logic Unit with addition/multiplication |
| **Magnitude Comparator** | `mag_comp.xpr` | Compares two binary numbers (>, <, =) |

### Display & Interface

| Project | File | Description |
|---------|------|-------------|
| **BCD to 7-Segment** | `BCD7seg.xpr` | Converts BCD input to 7-segment display patterns |
| **PWM LED Control** | `pwmLed.xpr` | Pulse-width modulation for LED brightness control |

### Combinational Logic

| Project | File | Description |
|---------|------|-------------|
| **4x1 Multiplexer** | `mux4x1.xpr` | 4-to-1 data selector circuit |
| **Bitwise Operations** | `bitwiseops.xpr` | AND, OR, XOR, NOT logic operations |

### Sequential Circuits

| Project | File | Description |
|---------|------|-------------|
| **Flip-Flops** | `flipflops.xpr` | D, T, JK, and SR flip-flop implementations |
| **Sequential Circuit** | `sqlckt.xpr` | State machine design practice |
| **Stop-Wait-Go** | `stopwaitgo.xpr` | Traffic light controller FSM |

### Signal Processing

| Project | File | Description |
|---------|------|-------------|
| **FIR Filter** | `FIRfilter.xpr` | 3-tap [1,2,1] digital FIR filter |
| **EPC** | `EPC.xpr` | Error correction/detection circuit |

### Application Projects

| Project | File | Description |
|---------|------|-------------|
| **Digital Safe System** | `digsafesystem.xpr` | 4-bit code verification security system |
| **Car Parking System** | `carpark.xpr` | Parking space counter/controller |
| **Test IP** | `testIP.xpr` | IP core testing and verification |
| **Parallel Practice** | `parapractice.xpr` | Parallel data processing exercises |

---

## Hardware Setup

| Component | Specification |
|-----------|---------------|
| **FPGA Board** | Digilent Basys-3 |
| **FPGA Chip** | Xilinx Artix-7 (XC7A35T-1CPG236C) |
| **Clock** | 100 MHz onboard oscillator |
| **Switches** | 16 slide switches for input |
| **Buttons** | 5 push buttons |
| **LEDs** | 16 user LEDs |
| **7-Segment** | 4-digit multiplexed display |

---

## Demonstrations

Video demonstrations of the projects running on hardware:

| Demo | Description |
|------|-------------|
| [ALU Demo 1](demos/videos/alu_demo_1.mp4) | Arithmetic operations demonstration |
| [ALU Demo 2](demos/videos/alu_demo_2.mp4) | Extended ALU functionality |
| [7-Segment Demo](demos/videos/seven_segment_demo.mp4) | Display multiplexing in action |
| [LED Counter](demos/videos/led_counter_demo.mp4) | Counter with LED visualization |

---

## Getting Started

### Prerequisites

- **Xilinx Vivado** 2023.x or later
- **Digilent Basys-3** FPGA board (for hardware testing)

### Opening Projects

1. Clone this repository:
   ```bash
   git clone https://github.com/DarkDragoXE/FPGA-Based-Mini-projects.git
   ```

2. Open Vivado and load any project:
   ```
   File -> Open Project -> projects/<project_name>.xpr
   ```

3. Generate bitstream and program the FPGA:
   ```
   Flow Navigator -> Generate Bitstream -> Program Device
   ```

---

## Project Structure

```
FPGA-Based-Mini-projects/
├── README.md
├── projects/               # Vivado project files (.xpr)
│   ├── 4bitadder.xpr
│   ├── fpgaALU.xpr
│   ├── FIRfilter.xpr
│   └── ... (17 projects)
├── demos/
│   └── videos/            # Hardware demonstration videos
│       ├── alu_demo_1.mp4
│       ├── alu_demo_2.mp4
│       ├── seven_segment_demo.mp4
│       └── led_counter_demo.mp4
└── images/                # Documentation images
    └── basys3_demo.jpeg
```

---

## Key Concepts Covered

| Category | Topics |
|----------|--------|
| **Combinational** | Adders, Multiplexers, Comparators, Logic Gates |
| **Sequential** | Flip-Flops, Counters, State Machines |
| **Arithmetic** | Binary Addition, Multiplication, ALU Design |
| **Signal Processing** | FIR Filtering, Digital Signal Processing |
| **I/O Interfacing** | 7-Segment Display, PWM, LED Control |
| **Applications** | Security Systems, Traffic Controllers |

---

## Toolchain

| Tool | Version | Purpose |
|------|---------|---------|
| **Xilinx Vivado** | 2024.1 | Synthesis, Implementation, Simulation |
| **Verilog HDL** | IEEE 1364-2005 | Hardware Description |
| **Basys-3 Board Files** | Latest | Constraint files and pin mapping |

---

## Author

**Debtonu Bose**  
Electronics and Communication Engineering  
VIT University

---

## Future Enhancements

- [ ] Add Verilog source files to repository
- [ ] Include testbenches for each module
- [ ] Add constraint files (.xdc)
- [ ] Create detailed documentation for each project
- [ ] Add simulation waveform screenshots

---

<div align="center">

**Learning digital design one gate at a time**

</div>
