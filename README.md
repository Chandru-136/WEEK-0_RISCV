## WEEK-0_Getting Started with Digital VLSI SOC Design , Planning and Tools Installation
The diagram illustrates the digital VLSI SoC design and planning flow, starting from chip modeling to final GDSII. The first stage (O1) involves defining specifications in a C model, with testbenches also written in C. Next, the RTL architect creates a soft copy of the hardware using Verilog RTL (O2). At this stage, the design is broken into major blocks such as processor, peripherals, and IPs. These are synthesized to gate-level netlists, synthesized macros, and functional analog IPs. The third stage (O3) focuses on SoC integration, where GPIOs and all subsystems are combined into a complete system-on-chip. After integration, physical design begins with floorplanning, placement, clock tree synthesis, and routing. Hardened macros and IP libraries are used during this phase. Finally, the design undergoes signoff checks such as DRC and LVS before generating the GDSII file, which is sent for fabrication, completing the RTL-to-GDS flow.

## Tool Installation Verification
# Yosys
![Yosys](https://github.com/Chandru-136/WEEK-0_RISCV/blob/main/images/gtkwave.png?raw=true)

# Iverilog
![Yosys](https://github.com/Chandru-136/WEEK-0_RISCV/blob/main/images/iverilog%20version.png?raw=true)


# GTKWave
![Yosys](https://github.com/Chandru-136/WEEK-0_RISCV/blob/main/images/gtkwave.png?raw=true)
