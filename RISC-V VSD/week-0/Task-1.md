# week0-task2
## RISC-V Program tools installation
### System Check
---
check the system requirments before getting started

- 6GB RAM, 50 GB HDD
- Operation system ex: 64xbit or 32xbit
- 4vCPU

### Installation of Virtual Machine for linux
---
- Download the VirtualMachine using the link below or search for the same in google.
- Link : https://www.virtualbox.org/wiki/Downloads
- - select the download file as per your system requirments
  - ex : windows or MacOs
- After downloading, run the installation file and run the default installation.
- The interface looks something like the image below
<img width="620" height="580" alt="image" src="https://github.com/user-attachments/assets/48ceec31-c206-415e-8c1f-3515b378ee32" />


### Ubuntu Downloading
---
- Download the latest ubuntu version from the official website
- Link : https://ubuntu.com/download/desktop
- Tip : Save the file in the same directory as the VM for ease of use

### Activation of Linex-Ubuntu interface
---
Now, Creating the new VM and select the storage disk (the more space available the best)
- After creating a machine, "[Optical drive] empty" in storage space
- click on that and select the ubuntu file we have just ownloaded
- now, run the machine. It will ask permissions and during the first time it will ask for account name, user name and password for the super user
- make sure you remember those
- follow the default steps and done. We have sucessfully installed the linex-ubuntu in windows using oracle VM.
- You will end up with a interface like the following image
  
  <img width="600" height="500" alt="Screenshot from 2025-09-19 18-43-37" src="https://github.com/user-attachments/assets/719d7769-9361-4c35-b377-a6632823c70a" />


## Resizing the Ubuntu window to fit the screen
```bash
$ sudo apt update
$ sudo apt install build-essential dkms linux-headers-$(uname -r)
$ cd /media/spatha/VBox_GAs_7.1.8/
$ ./autorun.sh
```
- if you still havent got it, try kunal sir udemy free course 
- link : https://www.udemy.com/course/vsd-a-complete-guide-to-install-open-source-eda-tools/


## Installation of Yosys
- Yosys is a open source tool used to RTL design and verification
- installing it is very easy
- open terminal in linex
- follow the prompted commands below

```bash
$ sudo apt-get update
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
# Yosys build depends on a Git submodule called abc, which hasn't been initialized yet. You need to run the following command before running make
$ git submodule update --init --recursive
$ make 
$ sudo make install
```
<img width="600" height="505" alt="image" src="https://github.com/user-attachments/assets/ff767ea7-3d35-42a0-89f7-15a287b0243c" />


## Installing iverilog
---
- iverilog is a open-source compiler and simulator that is used for digital electronics design and verification
- following the commands we can install the iverilog

```bash
$sudo apt-get install iverilog
```

<img width="651" height="500" alt="image (1)" src="https://github.com/user-attachments/assets/07077e4a-f668-4c63-ad55-142c7e994bf3" />

### Installing GTKWave
---

- GTKWave is a open-source to understand the wave-form viewer and debugger
- Use the command shown for installation of gtkwave

```bash
$sudo apt install gtkwave
```


<img width="763" height="100" alt="Screenshot from 2025-09-19 20-33-30" src="https://github.com/user-attachments/assets/c5a9a5c1-3f12-4da6-b1c1-71b8f139e335" />


<img width="602" height="546" alt="Screenshot from 2025-09-19 22-48-42" src="https://github.com/user-attachments/assets/703b8632-9135-4994-8658-63249fb206b5" />


## End Note
---
- I recmommend using the available gpt's if you have any doubts like gemini, chatgpt, grok and deepseek
- I highly recommend checking out **kunal ghosh** sir's udemy course for a neat and clear process of the installing of eda tools
  
### Acknowledgment 

- I want to thank **kunal ghosh ** sir for the amazing opportunity to be a part of RISC-V SoC Tapeout programme
- I also want to express my gratitude to **VSD** team for making this amazing opportunity available for all as a free course


