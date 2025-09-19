# VLSI Design Flow
---
- VLSI from specifications to tapeout has a variety of steps
- Those steps and in each and every step, all aims to obtain one result making the chip making and that is to maintain the same results as the desired specifications
- These steps consists of deciding the required specifications and compiling them through gcc to sending gdsii files to foundary for tapeout
- The steps include :
- - Specification
  - RTL Design
  - Physical design
  - TapeOut
## Specification
---
- These is the step that specifies the specific application
- This is done using a gcc compiler and checking that these specifications holds true
- Lets suppose **O0** is the output of the **gcc** and **O1** is the result of the application desired
- We have to make sure that **O0** and **O1** are always equal
## RTL Designing 
- Register Transfer Level (RTL) is a design abstraction in digital hardware design that describes how data moves between registers and the logic operations performed on that data within a digital system
- To design this the most popular HDL languages used are **Verilog** and **VHDL**
- The RTL design are then further devided / sliced into two parts
- - processor
  - - Synthesizable Gate Level Netlist
  - Pheriperals/IP
  - - Synthesizable macros
    - Functional Analog IPs
- Let the result of the RTL be **O2**
## Physical Design
- In physical design there consists of several steps which are :
- - Floor Planning
  - Placement
  - CTS
  - Routing
  - GDSii
- These steps are followed untill we have GDSii file
- Let the result of this be **O3**
## Foundary TapeOut
- During this stage, the GDSii file is then verified by the foundaries using **DRC/LVS** checks
- Let this result be **O4**

## Final Goal of VLSI FLOW

- The final result for a ideal chip is when we accuire **O0 == O1 == O2 == O3 == O4**
- It is to note that at every step, verification using different methodologies are performed to understand that the design hold the desired specifications


