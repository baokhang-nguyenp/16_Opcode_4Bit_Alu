# 16-Opcode 4-Bit ALU Design & Verification

**Student:** Nguyen Phuc Bao Khang (SE203511)
**Course:** Digital System Design Lab
**Software:** Vivado 

## Project Overview
This project features the RTL design and verification of a 4-bit Arithmetic Logic Unit (ALU) supporting 16 distinct operations. Unlike standard combinational designs, this ALU integrates a multi-cycle sequential unit to optimize hardware utilization.

## Key Features
- **16 Full Opcodes:** Exploits the entire 4-bit instruction space.
- **Modular RTL Architecture:** Utilizes separate sub-modules for Arithmetic, Logic, and Shift operations.
- **FSM-based MUL/DIV Block:** A Finite State Machine implements Shift-and-Add algorithms for multi-cycle multiplication and restoring division (with remainder), significantly reducing hardware area compared to combinational operators.
- **Exhaustive Verification:** A SystemVerilog self-checking testbench validates the design against a mathematical Golden Model across all 4,096 possible input combinations, confirming 0 errors.

## Hardware Utilization (Artix-7 FPGA)
- Slice LUTs: 75
- Slice Registers: 18

## Repository Structure
- `1_Source_Code/`: Verilog RTL design modules and SystemVerilog testbench.
- `2_Documents/`: Answer sheet report, Viva presentation slides, and 6 standardized Vivado flow screenshots.
- `3_Vivado_Project/`: Clean Vivado `.xpr` project file and `srcs` directory.

## Visual Flow
<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/0a1ad516-2484-4887-af99-81fc28c6d3a0" />

<img width="1918" height="1198" alt="image" src="https://github.com/user-attachments/assets/3ce4b614-dbe9-4814-a010-587f8df8d5c0" />
