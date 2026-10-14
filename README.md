# Multi-Cycle RISC-V Processor

## Overview

This project focuses on the design and implementation of a multi-cycle RISC-V processor using Verilog HDL.

Unlike a single-cycle architecture, the multi-cycle design divides instruction execution into multiple stages, allowing different instructions to take different numbers of clock cycles to complete.

The project explores the implementation of a multi-cycle datapath, control logic, and sequential instruction execution.

## Key Features

- Multi-cycle processor architecture
- Sequential instruction execution across multiple clock cycles
- Datapath and control unit implementation
- Instruction decoding and control signal generation
- Arithmetic and logical operations using the ALU
- Program Counter (PC) update logic
- Register file and immediate generation
- State-based control of processor operations

## Architecture

The processor is designed around the following components:

- **Program Counter (PC):** Stores the address of the current instruction.
- **Control Unit:** Coordinates instruction execution across multiple clock cycles.
- **Finite State Machine (FSM):** Controls the sequence of operations required to execute instructions.
- **Register File:** Stores general-purpose registers and provides source operands.
- **ALU:** Performs arithmetic and logical operations.
- **Immediate Generator:** Extracts and extends immediate values from instruction fields.
- **Datapath:** Transfers data between processor components during instruction execution.

## Instruction Execution

Instruction execution is divided into multiple clock cycles. Depending on the instruction, the processor may perform different sequences of operations.

Typical execution stages include:

1. Instruction Fetch
2. Instruction Decode and Register Fetch
3. Execute or Address Calculation
4. Memory Access, when required
5. Write Back, when required

The exact sequence and number of cycles depend on the implemented control logic and instruction type.

## Technologies

- **Hardware Description Language:** Verilog HDL
- **Instruction Set Architecture:** RISC-V
- **Processor Architecture:** Multi-Cycle

## Author

Amirhossein Mohammadi
