# Synthesis Flow using Yosys
---
## Introduction to Yosys

Yosys is a open-source synthesizer tool used to convert **RTl design** to **netlist**

- netlist is a representation of electronics devices in a code format
- this code is then used in physical design process
---
## Yosys flow
### Reading Liberty File
```bash
$ read_liberty -lib <lib file path> (../lib/sky file.lib)
```
---
### Reading Verilog file
```bash
$ read_verilog good_mux.v
```
---
### declaring top module
```bash
$ synth -top <module_name> (good_mux)
```
---
### ABC opertaion
```bash
$ abc -liberty <file_path to lib> (../lib/sky.lib)
```
---
### Synth design
```bash
$ show
```
---
![Image Alt](https://github.com/AS-Arshad/Repo1/blob/552b6107a99037ed52a4ee821cb9d6f943cb30b1/RISC-V%20VSD/week-1/Day-1/synth%20model.png)
