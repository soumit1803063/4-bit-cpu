# 4-Bit CPU Simulation with Digital Logic Design

This project showcases a fully functional 4-bit CPU, designed and simulated using digital logic circuits. The architecture includes essential components such as the Arithmetic Logic Unit (ALU), Control Unit (CU), Program Counter (PC), and registers, providing a foundational understanding of CPU operation and digital design principles.

## Building Process

The CPU is constructed through a series of interconnected components, where each subsequent component is built using the preceding ones:

1. **Arithmetic Units**:
   - **4BIT_FA.dig** is built using **1BIT_FA.dig**, creating a 4-bit full adder from 1-bit full adders.
   - **4BIT_SHL.dig** implements a shift-left circuit for bit manipulation.
   - **4BIT_XOR.dig** provides XOR functionality for logical operations.

2. **Registers**:
   - **4bitReg.dig** is constructed from **1bitReg.dig**, forming a 4-bit register.
   - **4bitregSetWith3regs.dig** integrates multiple **4bitReg.dig** instances into a functional set.

3. **Memory**:
   - **1x4ram.dig** is developed from **1x1ram.dig**, leading to **1x16ram.dig**, which is further expanded into **9x16ram.dig**, creating a hierarchical RAM structure that progressively increases in capacity and width.

4. **Control and Execution**:
   - **4bitPC ADDER.dig** implements the program counter adder to manage instruction fetching.
   - **4bitProgramCounter.dig** constructs the program counter using prior components.

5. **Core Functionality**:
   - **ALU.dig** serves as the computational heart of the CPU, handling arithmetic and logic operations.
   - **CU.dig** is the control unit that orchestrates the operation of the CPU.
   - **4bitCPU.dig** integrates all components into a complete CPU system.

## Features

- **Modular Design**: Each CPU component is created as a standalone `.dig` file, allowing for individual testing and enhancements.
- **Educational Resource**: Ideal for students and educators to understand CPU architecture and digital logic design principles.
- **Documentation**: Accompanied by a detailed PDF document (18CT4Doc_1803063.pdf) that outlines the design, component functions, and overall architecture.

## Getting Started

Clone the repository and utilize a digital circuit simulation tool (e.g., Logisim) to open and explore the `.dig` files. Each file is designed to be standalone and can be tested independently.

## Future Work

Potential extensions may include expanding the architecture to an 8-bit CPU, adding more complex instruction sets, or integrating I/O modules for enhanced functionality.

---

This project provides a comprehensive introduction to digital logic and CPU design, making it suitable for those interested in the fundamentals of computing architecture.
