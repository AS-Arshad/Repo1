# Introduction to RTL design and Synthesis

In this repo we are going to understand the very basic terms and tool associated

## Introduction to Simulators

Simulators are the tools that check whether the RTL design generated through HDL is still equivalent to the specifications (specs) desired/intended

- simulators check whether the design is still maintaining the intended functionality
- we can understand that the design is still holiding the functionalities of the intended specs only after the results from the simulators
- The simulators overview can be understood by the following figure :

![Image Alt](https://github.com/AS-Arshad/Repo1/blob/aabc4ce56cfe73d857b68faca0b006f6d464248b/RISC-V%20VSD/week-1/Day-1/Screenshot%20from%202025-09-24%2021-04-44.png)


---- Now lets go over each thing

## Design 
- It is the description of the specification in HDL format (ex. Verilog or VHDL etc)
- The design is prompted to maintain the desired specs
- The design consists of primary inputs and primary outputs
- - these are the i/o pins used to connect to the design (there can be many internal connections which are called wires and we are not talking about those)
- Now to check whether the design actually following the intended specs, we need a test-bench to authenticate the design


## Test-Bench
- Test-bench is a setup to stimulate the input values (input vectors) through the design and understand the outputs the design generates are matching the intended specs or not
- There are a large variety of input vectors we can provide to a design through the test-bench
- Test-bench consists of **stimulus generator** and a **stimulus observer** which are the main functions of the testbench
- these generates the test vectors and identify if there are any deviations in the output from the intended specs
- **Important to note** : Test-bench doesnot contains any input or output values
- It stimulates the design using different input vectors and helps us understand whether the design is producing the similar results as the intened specs
- Now, where and how we can write and simulate the design using test-bench setup ?
- - we use simulators to do the work
  - We are going to understand the simulation flow with the help of open-source toll **iverilog**
 
## iverilog

- it is a open-source simulator tool used to verify the design
- iverilog performs the simulation by feeding the test stimulus from testbench to design and checking the resulted output
