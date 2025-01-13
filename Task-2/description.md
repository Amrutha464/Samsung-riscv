# Task 2 - SPIKE Simulation and Optimization Flags

## Description
This repository contains the results of running the **sum_1ton** program on the **SPIKE** RISC-V simulator with two different compiler optimization flags: `-O1` and `-Ofast`. The task involved compiling the **sum_1ton** program with the **RISC-V GCC** toolchain, running the simulation to observe performance under both optimization levels, and collecting the corresponding **RISC-V object dumps** for each optimization.

## Files Included:
- **sum_1ton_O1.dump**: Object dump file generated after compiling with the `-O1` compiler optimization.
- **sum_1ton_Ofast.dump**: Object dump file generated after compiling with the `-Ofast` compiler optimization.
- **SPIKE Simulation Output**: Logs and results from running the **sum_1ton** program on the **SPIKE** RISC-V simulator under both optimization flags.

## Steps Performed:
1. **Write the sum_1ton Program**  
   A simple C program that calculates the sum of integers from 1 to N.
   
2. **Compile the Program with the RISC-V GCC Toolchain**  
   The **sum_1ton** program was compiled under two different optimization levels:
   - **`-O1`**: Basic optimizations with moderate focus on debugging.
   - **`-Ofast`**: Aggressive optimizations for performance at the cost of debugging.

3. **Run the Program Using the SPIKE RISC-V Simulator**  
   After compiling the program, the generated binary was run on the **SPIKE** simulator with the **pk (proxy kernel)** to emulate RISC-V architecture and observe the program's performance under both optimization flags.

4. **Generate the RISC-V Object Dump for Each Optimization Level**  
   Object dumps for both optimization levels (`-O1` and `-Ofast`) were generated using **riscv64-unknown-elf-objdump**, providing assembly-level details for each version of the program.

5. **Upload the Results to GitHub**  
   The following files were uploaded to this repository:
   - The object dumps for both optimization levels (**sum_1ton_O1.dump**, **sum_1ton_Ofast.dump**).
   - The **SPIKE simulation logs** showing the program's execution results for each optimization level.

## Instructions to Replicate the Process:

1. **Compile the C Program**  
   Use the **RISC-V GCC toolchain** to compile the **sum_1ton** program for each optimization level (`-O1` and `-Ofast`).

2. **Run the Program on the SPIKE Simulator**  
   After compilation, run the program using the **SPIKE** RISC-V simulator with the **proxy kernel** (pk) to simulate execution.

3. **Generate the Object Dumps**  
   Use the **riscv64-unknown-elf-objdump** tool to generate the object dumps for both optimization levels.

4. **Update Your GitHub Repository**  
   Add the **sum_1ton.c** source code, the object dumps, and the **SPIKE simulation logs** to this repository.

