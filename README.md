 AMBA AXI4 Interconnect Using Verilog HDL

Project Description

As modern System-on-Chip (SoC) designs become increasingly complex, a reliable communication interface is essential for connecting processors with memory and peripheral devices. This project focuses on designing and implementing an **AMBA AXI4 Interconnect** using **Verilog HDL**, providing a simple yet efficient communication path between a single AXI master and multiple AXI slave modules.

The objective of this project was to understand the AXI4 protocol in depth and implement its fundamental concepts through a modular hardware design. The interconnect receives read and write requests from the master, decodes the target address, and forwards each transaction to the appropriate slave. An **Address Decoder** is used to identify the destination peripheral, while a **Cache Memory Controller** and a **FIFO** are integrated as the two AXI slave modules.

Each module was designed independently and then integrated into the top-level architecture to ensure proper communication between the master and the slaves. Functional verification was carried out using dedicated Verilog testbenches to validate different read and write scenarios. After successful RTL verification, the design was synthesized and implemented using **Synopsys Design Compiler** and **IC Compiler II**, following a standard ASIC design flow.

Developing this project provided valuable practical experience in RTL design, digital system integration, verification, synthesis, timing analysis, and physical implementation. It also strengthened my understanding of on-chip communication protocols and how modular hardware components work together in real-world SoC architectures.

This project serves as a strong foundation for learning advanced AMBA protocols and can be extended in the future by supporting multiple masters, additional slave peripherals, burst transaction optimization, arbitration mechanisms, and Quality of Service (QoS) features.

 Key Features

* Designed using Verilog HDL
* Implements an AMBA AXI4-based interconnect architecture
* Single AXI Master communicating with multiple AXI Slaves
* Address-based routing through an Address Decoder
* Cache Memory Controller integrated as Slave 1
* FIFO integrated as Slave 2
* Modular and reusable hardware design
* Functional verification using Verilog testbenches
* Synthesized and implemented using Synopsys EDA tools

Project Structure
AMBA_AXI4_Interconnect/
├── RTL/
│   ├── axi_master.v
│   ├── axi_interconnect.v
│   ├── address_decoder.v
│   ├── cache_memory_controller.v
│   ├── fifo.v
│   └── axi4_interconnect_top.v
│
├── Testbench/
│   └── tb_axi4_interconnect.v
│
├── Constraints/
│   └── axi4_interconnect.sdc
│
├── Synthesis/
|      (Generation of gate-level-netlist)
│
|── DFT/
|      (design for testability- modules are tested using design compiler shell(dc_shell)
|
├── Physical_Design/
|      (Floorplanning, routing, etc..,)
│
├── Results
       (GDSII generation)

Tools and Technologies

* Verilog HDL
* Synopsys Design Compiler
* Synopsys IC Compiler II
* Static Timing Analysis (STA)
* ASIC Design Flow

Applications

The concepts implemented in this project are widely used in modern ASIC and FPGA designs, including embedded systems, automotive electronics, communication devices, networking hardware, consumer electronics, and System-on-Chip (SoC) architectures where efficient data transfer between processing units and peripherals is required.

 About This Project

This project was developed as part of my learning journey in VLSI and ASIC design. The goal was not only to implement an AXI4 Interconnect but also to gain hands-on experience with the complete digital design flow, from RTL development and functional verification to synthesis and physical implementation using Synopsys tools. It reflects my practical understanding of hardware design principles and my interest in SoC architecture and digital system design.
