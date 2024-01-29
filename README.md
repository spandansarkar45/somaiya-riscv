# VSD RISC-V Internship Program
## Day 1-Introduction to RISC-V ISA And GNU compiler toolchain
### RISC-V ISA (Reduced Instruction Set Computing Five):

Open-Source Architecture: RISC-V is an open-source ISA, offering transparency and fostering collaborative development.
Modular Design: Emphasizes simplicity and modularity, allowing for flexible and efficient processor implementations.
### GNU Compiler Toolchain for RISC-V:

Cross-Platform Development: Supports software development for RISC-V architectures, ensuring portability across diverse systems.
Code Optimization: The toolchain, including GCC (GNU Compiler Collection), employs advanced optimization techniques to enhance code efficiency.
### Example RISC-V Instructions:
<br> Pseudo instructions - For e.g- mv,li,ret etc
<br> Base integer instruction (RV64I, RV32I)-For e.g-lui,addi etc
<br> Multiply extension (RV64M) -For e.g- mulw,divw etc
<br> Single and double floating point instruction (RV64F, RV64D) -For e.g- flw,fadd etc
<br> Application binary instruction
<br> Memory allocation and stack pointer

## Labwork for RISC-V Software Toolchain

### C Program to compute sum from 1 to n
Following is the input code for the program on Text Editor :
![Sum1ton c (Input)](https://github.com/spandansarkar45/somaiya-riscv/assets/154997186/f1a83442-9f8d-4fd7-8886-4cf6e4e0dab2)
Following is the output for the program on Terminal Window :
![Sum1ton c (Output)](https://github.com/spandansarkar45/somaiya-riscv/assets/154997186/fe328267-4287-4ba7-8c3f-34afc761b10d)

### RISC-V GCC Compile and Disassemble
The following terminal tab denotes the input code for the C compiler but now our task is to obtain the assembly codes for the C program using RISC-V Simulator. The commands used are for generating an object file i.e 'Sum1ton.o' :
![RISC-V Simulator](https://github.com/spandansarkar45/somaiya-riscv/assets/154997186/a56dc5ae-d490-4318-97d4-af0ae2201b7e)
The next tab denotes the object dump disassemble commands for Sum1ton.o :
![Objdump dis cmds](https://github.com/spandansarkar45/somaiya-riscv/assets/154997186/fb9d8dbb-61f2-40a4-a018-3112bd74da2c)

After executing the objdump commands, we find the Assembly code for the C program. To find the main section, type :
<br> /main (Enter)
<br> n (Enter)

Below is the Main Section of Assembly codes :
![As co Main Sec](https://github.com/spandansarkar45/somaiya-riscv/assets/154997186/461a0855-b501-4e23-8416-0ce8adcc1f7b)
Address of main section is 10184




