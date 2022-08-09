# 8-bit_CPU
### This is a simple, single-cycle, 8-bit CPU with 256 bytes of RAM built in Logisim.

## Overview:<br>
Uses Harvard computer architecture.<br>
https://www.geeksforgeeks.org/harvard-architecture/<br>
https://www.geeksforgeeks.org/difference-between-von-neumann-and-harvard-architecture/<br>

<b>There are eight 8-bit registers:</b><br>
One is a constant zero.<br>
Seven are writable.<br>

<b>Instructions are 20-bits, with two different instruction formats:</b><br>
R-Type (0): 19 (type), 18-14 (operation code), 13-9 (5-bit immediate), 8-6 (rt register), 5-3 (rs register), 2-0 (rd register)<br>
I-Type (1): 19 (type), 18-14 (operation code), 13-6 (8-bit immediate), 5-3 (rs register), 2-0 (rd register)<br>

<b>Arithmetic Logic Unit (ALU) operations:</b><br>
Addition and subtraction. Bitwise and, or, xor, not, shift left, shift right.<br>

<b>Control Flow:</b><br>
Jumps: jump, jump register, jump and link.<br>
Branches: if less than, if greater than or equal to, if equal, if not equal.<br>

<b>Output:</b><br>
Display: There are 4 faux-LED outputs that can display the digits 0x0000 through 0xFFFF (65,535 in decimal).<br>
Teletype: Contains a functional TTY that works with a specific program that can be loaded into the ROM.<br>

The Logisim file in this repository contains the complete and fully-functional project with a program to display prime numbers (in hexadecimal) loaded into the ROM.<br>

Pictures of the main and sub-circuits are below.<br>

## Main Circuit
![cpu-main](https://user-images.githubusercontent.com/97967500/183528661-1ba10934-1b90-4174-b010-823f32e826ce.png)

## Display Circuit
![cpu-display](https://user-images.githubusercontent.com/97967500/183530020-bbf1220e-b0c8-4843-b36f-a610e0faf3b1.png)

## Arithmetic Logic Unit Circuit
![cpu-ALU](https://user-images.githubusercontent.com/97967500/183530075-7ec20816-0b31-4aa8-8668-58dc230cc4f0.png)

## Register File Circuit
![cpu-regFile](https://user-images.githubusercontent.com/97967500/183530085-48e12af9-31bc-4010-ab16-450b60a2febc.png)

## Program Counter Circuit
![cpu-programCounter](https://user-images.githubusercontent.com/97967500/183530332-a8374f60-4157-4160-a169-52ac0b1cb555.png)

## Control Circuit
![cpu-control](https://user-images.githubusercontent.com/97967500/183530117-aec396bf-a043-41dc-a2ca-6df93c71a458.png)
