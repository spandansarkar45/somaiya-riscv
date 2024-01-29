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

## Integer Number Representation

### 64 bit Number System for Unsigned Numbers
In the context of RISC-V, a 64-bit number system for unsigned numbers refers to the representation and manipulation of non-negative integers using 64 bits. Each bit in the 64-bit binary number holds a specific place value, and the value of the entire 64-bit number is the sum of these place values.

For example, a 64-bit unsigned binary number might look like this:

\[ 1001011010100110101101101011010111010010110010101101110101010101 \]

In this binary representation, each digit is a bit (either 0 or 1), and the rightmost bit represents the least significant bit (LSB), while the leftmost bit represents the most significant bit (MSB).

With 64 bits, the range of representable unsigned integers is \(0\) to \(2^{64} - 1\), providing a wide numerical range for applications such as high-performance computing, data processing, and various embedded systems. The use of 64-bit unsigned numbers in RISC-V architectures allows for handling large and positive integer values efficiently.

![Unsigned numbers](https://github.com/spandansarkar45/somaiya-riscv/assets/154997186/8c6533a7-e2e9-4cca-aae1-945b575fe70c)

### 64 bit Number System for Signed Numbers
In the context of RISC-V, a 64-bit number system for signed numbers refers to the representation and manipulation of both positive and negative integers using 64 bits. The system typically follows the Two's complement representation for signed integers, where the most significant bit (MSB) is the sign bit (0 for positive, 1 for negative).

For example, a 64-bit signed binary number might look like this:

\[ 1101101010100110101101101011010111010010110010101101110101010101 \]

In this representation, the leftmost bit is the sign bit, and the remaining 63 bits represent the magnitude of the number. The Two's complement representation simplifies arithmetic operations by treating addition and subtraction uniformly.

With 64 bits, the range of representable signed integers is \(-2^{63}\) to \(2^{63} - 1\), providing a broad numerical range for various computing applications. The use of 64-bit signed numbers in RISC-V architectures allows for efficient handling of both positive and negative integer values in computations.




