# Digital Logic and Computer Organization

[中文](README.md) | [English](README-English.md)

This repository organizes learning materials about digital logic, computer organization, computer hardware design, and assembly language fundamentals. The content is based on the PDF and DOCX materials in `docs/` and is suitable for studying digital logic, CPU fundamentals, and embedded-system foundations.

## Materials

- [Digital Logic and Computer Organization PDF](docs/数字电路基础与计算机组成.pdf)
- [Digital Logic and Computer Organization DOCX Source](docs/数字电路基础与计算机组成.docx)

## Learning Roadmap

```text
Digital logic fundamentals
    ├── Binary data representation
    ├── Basic logic gates and combinational logic
    ├── Arithmetic units
    ├── Latches, flip-flops, and registers
    └── Digital circuit simulation
            ↓
Computer organization
    ├── Von Neumann model
    ├── CPU, memory, and I/O
    ├── Program execution
    └── A simple computer
            ↓
Computer hardware design
    ├── ALU and calculation unit
    ├── Data and instruction storage
    ├── Control signals and controller
    ├── RAM, PC, and instruction register
    └── Fetch, decode, and execute
            ↓
Assembly, buses, and boot programs
    ├── Custom instruction set and assembly programs
    ├── Bus and address mapping
    └── Boot flow and microcontroller startup
```

## Contents

### Chapter 1: Digital Logic Fundamentals

- Understand binary numbers, bits, bytes, and data units.
- Learn how text, images, sound, and video can be represented in binary.
- Use the Digital simulator to observe digital circuit behavior.
- Learn AND, OR, NOT, and other basic logic gates.
- Understand the basic structure of arithmetic and combinational logic.
- Study SR latches, D latches, and edge-triggered D flip-flops.
- Understand the role of registers in data storage and sequential circuits.

### Chapter 2: Computer Organization

- Understand the basic structure of a Von Neumann computer.
- Learn the responsibilities of the CPU, memory, and input/output system.
- Understand how a program is stored and executed.
- Compare the characteristics of different computer architectures.
- Understand how computation, storage, control, and I/O form a simple computer.

### Chapter 3: Computer Hardware Design

This chapter develops a simple computer step by step, with emphasis on the datapath, control signals, and instruction execution.

- Implement an ALU and a simple calculation unit.
- Use registers for data storage and connect external data memory.
- Add instruction storage and a program counter (PC).
- Add control instructions such as `halt`, `str`, `ld`, `jmp`, `cmp`, and `je`.
- Add data-selection and register-control signals such as `enA`, `selA`, and `selB`.
- Design a controller and maintain its control-signal lookup table.
- Combine instruction storage and data storage into a unified RAM.
- Understand instruction fetch, instruction execution, and timing-state transitions.
- Add immediate values and a B register.
- Validate the instruction set and hardware circuit with test programs.

### Chapter 4: Designing an Assembly Language

- Write assembly programs for the custom instruction set.
- Use load, arithmetic, jump, comparison, and save instructions to build program flow.
- Test the execution result of assembly programs on the custom computer with examples such as summation.

### Chapter 5: Bus and Input/Output Design

- Understand data exchange between the CPU circuit and external devices.
- Learn the purpose and basic structure of a bus.
- Understand bus address mapping and how the CPU accesses different memory and I/O devices.

### Chapter 6: Boot Program Design

- Understand the boot flow after a computer is powered on.
- Design initialization, loading, and control-flow transfer.
- Use programs to load stored data and perform control-flow jumps.
- Connect microcontroller boot flows with the startup process of general-purpose computers.

### Chapter 7: Common Digital ICs

- AND, OR, and NOT gates.
- `74HC245N`: buffer, bus transceiver, and driver.
- `74HC138`: decoder.
- `DS1302`: real-time clock IC.

## Core Concepts

| Concept | Role |
| --- | --- |
| Bit | The smallest data unit representing `0` or `1` |
| Byte | Usually composed of 8 bits |
| Logic gate | Performs logic operations on binary signals |
| Latch | Stores data while an enable condition is active |
| Flip-flop | Stores a state on a clock edge |
| Register | Sequential circuit that stores multiple bits |
| ALU | Performs arithmetic and logic operations |
| PC | Program counter holding the address of the next instruction |
| RAM | Read/write storage for data or instructions |
| Control unit | Generates control signals from instructions |
| Bus | Shared transmission path connecting CPU, memory, and I/O |
| Instruction set | The instructions a computer can recognize and execute |

## Instruction Set Evolution

The custom computer in the course material is extended in the following sequence:

```text
Basic addition and subtraction
    ↓
halt
    ↓
str and ld
    ↓
Logic operations and register selection
    ↓
jmp
    ↓
cmp and je
    ↓
Unified RAM and fetch/execute cycles
    ↓
Immediate values
    ↓
B register and a more complete instruction set
    ↓
Assembly programs and boot programs
```

## Suggested Study Process

1. Learn binary numbers, logic gates, truth tables, and basic sequential circuits first.
2. Use the Digital simulator to trace every input, output, and control signal.
3. When studying CPU design, record the datapath, control path, clock state, and instruction format separately.
4. For each instruction, track its opcode, operands, register changes, and memory changes.
5. Start with simple test programs, then verify jumps, immediate values, registers, and I/O features.

## Directory Structure

```text
digital-logic-and-computer-organization/
├── README.md
├── README-English.md
└── docs/
    ├── 数字电路基础与计算机组成.pdf
    └── 数字电路基础与计算机组成.docx
```

## Current Scope

The repository currently focuses on the course PDF, DOCX source, and learning index. It does not include additional Digital circuit files, simulation projects, assembler implementations, or execution logs. Future work can add these materials by chapter.

## Keywords

`Digital Logic` `Computer Organization` `CPU` `ALU` `RAM` `Register` `Instruction Set` `Assembly Language` `Bus` `I/O` `Digital Circuit Simulation`
