# Simulation iverilog

- executing a mux using iverilog
- using the correcponding testbench
- running the iverilog simulator
- debugging using gtkwave

## Exection

- we are taking the good_mux.v file which is already available from sky directory
- the execution can be done by following prompts :
![Image Alt](https://github.com/AS-Arshad/Repo1/blob/61c4843e8f521c6288d952468d9c183bb8399c61/RISC-V%20VSD/week-1/Day-1/iverilog%20execution.png)


### Simulation using iverilog

- lets go through the execution

- we have performed the simulation using **iverilog**

```bash
$ iverilog good_mux.v tb_good_mux.v
```
- the prompt will simulate the design **good_mux.v** using test-bench **tb_good_mux.v**
- the simulator is **iverilog**
- now as stated in previous notes, the simulator uses design and tb files to generate a **.vcd** file

**Now checking the directory we can now see a **a.out** file present in the directory**

- we are now executing the **a.out** file

  ```bash
  $ ./a.out
  ```

  - we can see that the files are dumped and created a new file **good_mux.vcd**
 
  - Using this file we can observe the waveform using gtkwave
  - the observed wave form can be understand in the following picture :

    ![Image Alt](https://github.com/AS-Arshad/Repo1/blob/26317e5e5bce843ef3150003d7cd0675f9d8c422/RISC-V%20VSD/week-1/Day-1/good_mux%20waveform%20using%20gtkwave.png)
 
  
