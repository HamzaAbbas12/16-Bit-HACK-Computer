### 16-bit Hack Computer Design | *Hardware Description Language (HDL), Digital Logic, Computer Architecture*



![image](https://github.com/user-attachments/assets/9311ad8b-5a4e-48bc-af58-121114ba3e99)

Hack Computer Diagram, as specified by NANDtoTetris

**Jan. 2024 – May 2024**



This project showcases the design and implementation of a fully functional 16-bit Hack Computer, built from scratch using fundamental digital logic principles. At the heart of this system is a **Central Processing Unit (CPU)** capable of decoding and executing Hack assembly instructions, controlling the flow of data and operations between the **Arithmetic Logic Unit (ALU)** and **Memory**. This project, constructed as part of the renowned "NAND to Tetris" course, demonstrates deep knowledge of digital design, computer architecture, and hardware-software integration.

### Modular Design Approach (Bottom-Up)

The development of the Hack Computer followed a **bottom-up design methodology**, where the most basic components were first constructed, and progressively more complex structures were built on top of them. This hierarchical approach ensured a strong foundational understanding of digital systems and their integration into a complete computational machine.

- **Basic Logic Gates:** Starting with NAND gates, I developed fundamental logic gates (AND, OR, NOT) used in all digital circuits.
- **Adders and ALU:** I designed half-adders and full-adders to create the 16-bit ALU, which performs essential arithmetic and logic operations.
- **Registers:** 16-bit data registers were implemented to store values and facilitate memory access during program execution.
- **RAM (Random Access Memory):** Using multiplexers and registers, I developed the RAM units that allow dynamic storage of data, enabling the execution of more complex instructions.
- **Program Counter:** I implemented a program counter to track the current instruction being executed, advancing or jumping based on conditional logic.
- **Integrated System:** These components were then integrated to form the CPU, ALU, and Memory, culminating in a fully functional computer capable of running Hack assembly code.

---

### Major Components:

### 1. Central Processing Unit (CPU)

![image](https://github.com/user-attachments/assets/331952d5-6c35-4043-87b5-fe9cfc543924)


CPU Diagram from NANDtoTetris

The **CPU** serves as the control center of the Hack Computer, responsible for interpreting Hack assembly instructions and directing the necessary operations. It integrates both combinational and sequential logic to handle decision-making, instruction sequencing, and data management.

- **Instruction Decoding and Execution:** The CPU interprets Hack assembly instructions, using control signals to manage operations such as arithmetic processing, logical comparisons, and memory access.
- **Combinational Logic:** Facilitates real-time data processing and immediate responses to input signals.
- **Sequential Logic:** Controls the flow of instructions and manages the state changes required for executing multi-step operations.

Major file associated: `CPU.hdl`

### 2. Arithmetic Logic Unit (ALU)

The **ALU** performs the core arithmetic and logical operations required by the Hack Computer, handling 16-bit data for operations like addition, subtraction, and bitwise manipulation.

- **Operations Supported:** Provides essential arithmetic (addition, subtraction) and logic (AND, OR, NOT) operations.
- **Flags for Decision-Making:** Outputs status flags (zero, negative) used by the CPU to determine program flow and conditional execution.
- **Data Inputs/Outputs:** Processes two 16-bit inputs and outputs a single 16-bit result, making it central to the computer's computational performance.

Major file associated: `ALU.hdl`

### 3. Memory Module

The **Memory** module manages the storage and retrieval of both program instructions and data during execution, with a division into **RAM** (for variable storage) and **ROM** (for program instructions).

- **RAM (Random Access Memory):** Temporary storage for variables, intermediate calculations, and program states.
- **ROM (Read-Only Memory):** Stores the machine-level instructions of the program executed by the CPU.
- **Control Logic:** Coordinates data transfer between the CPU and Memory, ensuring proper read/write operations.

Major file associated: `Memory.hdl`

### Project Complexity:

This 16-bit Hack Computer project highlights key concepts in **combinational** and **sequential logic design**, **memory management**, and the implementation of an **instruction set architecture** (ISA). The CPU, ALU, and Memory modules work in harmony to execute complex programs, all designed using HDL and tested through Hack assembly code.

![image](https://github.com/user-attachments/assets/9b9c2b8e-4b90-408a-856f-ae4d84f5db4e)

NANDtoTetris Hardware Simulator

### Technologies and Skills:

- **Hardware Description Language (HDL):** Designed and implemented the CPU, ALU, and Memory modules.
- **Instruction Set Architecture (ISA):** Implemented Hack's ISA, enabling the CPU to decode and execute a range of instructions.
- **Memory Management:** Developed RAM and ROM modules to handle dynamic data storage and fixed instruction sets.
- **Digital Logic Design:** Built from basic logic gates (NAND, AND, OR) to complex components.
- **Embedded Systems:** Applied low-level hardware and software knowledge to create a functional computer system.

### Key Accomplishments:

- Designed a fully operational 16-bit computer capable of executing Hack assembly programs.
- Demonstrated proficiency in CPU architecture, ALU design, and memory hierarchy.
- Applied HDL and digital logic concepts to create a real, working computational system.

### Course Credit:

This project was developed as part of the "NAND to Tetris" course, providing a hands-on experience in building a computer from the ground up, starting with logic gates and culminating in a functional machine capable of executing software programs.
