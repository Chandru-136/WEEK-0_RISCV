## WEEK-0_Getting Started with Digital VLSI SOC Design , Planning and Tools Installation
The diagram illustrates the digital VLSI SoC design and planning flow, starting from chip modeling to final GDSII. The first stage (O1) involves defining specifications in a C model, with testbenches also written in C. Next, the RTL architect creates a soft copy of the hardware using Verilog RTL (O2). At this stage, the design is broken into major blocks such as processor, peripherals, and IPs. These are synthesized to gate-level netlists, synthesized macros, and functional analog IPs. The third stage (O3) focuses on SoC integration, where GPIOs and all subsystems are combined into a complete system-on-chip. After integration, physical design begins with floorplanning, placement, clock tree synthesis, and routing. Hardened macros and IP libraries are used during this phase. Finally, the design undergoes signoff checks such as DRC and LVS before generating the GDSII file, which is sent for fabrication, completing the RTL-to-GDS flow.

## Tool Installation Verification
# Yosys
Yosys is a popular open-source framework for RTL synthesis. It takes Verilog HDL as input and generates gate-level netlists that can be mapped to ASIC standard cells or FPGA fabrics. Yosys supports a wide range of optimization techniques, including logic minimization, constant propagation, and technology mapping. It is the backbone of many open-source digital design flows such as OpenLane and integrates seamlessly with standard libraries like SkyWater 130nm PDK. With its extensible architecture, Yosys allows developers to experiment with synthesis algorithms and custom passes, making it an invaluable tool for education, research, and real-world VLSI design projects.
![Yosys](https://github.com/Chandru-136/WEEK-0_RISCV/blob/main/images/yosys.png?raw=true)

# Iverilog
With iverilog, you can run testbenches to verify that the Verilog code behaves as expected before synthesis. It produces output files that can be analyzed with tools like GTKWave for signal waveform visualization. Being lightweight, free, and widely supported, Icarus Verilog is especially useful for learning digital design, rapid prototyping, and academic research in VLSI and FPGA development.
Icarus Verilog, often called iverilog, is an open-source tool for compiling and simulating Verilog hardware description language (HDL). It allows designers to model, test, and debug digital circuits at the Register Transfer Level (RTL). 
![Iverilog](https://github.com/Chandru-136/WEEK-0_RISCV/blob/main/images/iverilog%20version.png?raw=true)


# GTKWave
GTKWave is a waveform viewer used to analyze and debug digital circuit simulations. It works by reading dump files (VCD, FST, LXT, etc.) generated during simulation with tools like Icarus Verilog. The tool provides a graphical interface to view and trace signal activity across time, helping designers confirm whether the design functions correctly. GTKWave supports advanced features such as hierarchical browsing, signal grouping, zooming, and search, making it efficient for large projects. Its simplicity and open-source nature make it a standard companion for Verilog/VHDL simulation, enabling engineers and students to validate logic functionality effectively during hardware development.
![GTKWave](https://github.com/Chandru-136/WEEK-0_RISCV/blob/main/images/gtkwave.png?raw=true)
