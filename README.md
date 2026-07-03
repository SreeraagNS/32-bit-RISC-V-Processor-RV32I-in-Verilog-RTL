# RISC-V 32-bit Single Cycle Processor

A 32-bit Single Cycle RISC-V Processor designed in Verilog HDL and implemented using Xilinx Vivado. This project demonstrates the implementation of the RV32I instruction set architecture with separate instruction and data memories, ALU, register file, control unit, and datapath.

## Features

- RV32I Instruction Set Support
- Single Cycle Datapath
- 32-bit ALU
- Register File (32 × 32-bit Registers)
- Immediate Generator
- Control Unit
- ALU Control Unit
- Program Counter
- Instruction Memory
- Data Memory
- Branch and Jump Instructions
- Load and Store Instructions
- Synthesizable Verilog Design

## Supported Instructions

- R-Type
  - ADD
  - SUB
  - AND
  - OR
  - XOR
  - SLL
  - SRL
  - SRA
  - SLT

- I-Type
  - ADDI
  - ANDI
  - ORI
  - XORI
  - LW
  - JALR

- S-Type
  - SW

- B-Type
  - BEQ
  - BNE
  - BLT
  - BGE

- U-Type
  - LUI
  - AUIPC

- J-Type
  - JAL

## Project Structure

```
.
├── rtl/
│   ├── top_riscv.v
│   ├── datapath.v
│   ├── control_unit.v
│   ├── alu.v
│   ├── alu_control.v
│   ├── register_file.v
│   ├── instruction_memory.v
│   ├── data_memory.v
│   ├── immediate_generator.v
│   └── ...
│
├── simulation/
│   ├── top_tb.v
│   └── test_program.mem
│
├── constraints/
│   └── *.xdc
│
└── README.md
```

## Datapath Overview

The processor consists of:

- Program Counter (PC)
- Instruction Memory
- Control Unit
- Register File
- Immediate Generator
- ALU
- Data Memory
- Branch and Jump Logic
- Write Back Multiplexer

All instructions execute in a single clock cycle.

## Simulation

The design can be simulated using:

- Xilinx Vivado Simulator
- ModelSim
- QuestaSim

Run the provided testbench (`top_tb.v`) to verify processor functionality.

## Synthesis

The processor has been synthesized using:

- Xilinx Vivado

Target FPGA can be modified by updating the project constraints.

## Tools Used

- Verilog HDL
- Xilinx Vivado
- Xilinx Simulator

## Future Improvements

- Five-Stage Pipeline
- Hazard Detection Unit
- Forwarding Unit
- Branch Prediction
- Instruction Cache
- Data Cache
- CSR Support
- Interrupt Handling

## Learning Outcomes

This project helped in understanding:

- Computer Architecture
- RISC-V ISA
- Processor Datapath Design
- Control Unit Design
- RTL Design using Verilog
- FPGA Synthesis and Simulation

## Author

**Sreeraag N S**

Applied Electronics and Instrumentation Engineering  
College of Engineering Trivandrum (CET)

---

⭐ If you found this project useful, consider starring the repository.
