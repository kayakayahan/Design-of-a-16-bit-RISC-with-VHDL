# Design-of-a-16-bit-RISC-with-VHDL
Using VHDL design a 16 bit RISC Processor


The system works with every two clock signal. 

Opcode:
Data Processing Instructions
0000 -- ADD, $R1 = $R1 + $R2
0001 -- SUB, $R1 = $R1 - $R2
0010 -- MUL, $R1 = $R1 * $R2
0011 -- SLA , $R1 = $R1 << 1
0100 -- SRA , $R1 = $R1 >> 1
0101 -- XOR, $R1 xor $R2
0110 -- AND, $R1 =$R1 and $R2
0111 -- Addi, $R1 = $R1 + $R3
1000 -- subi, $R1 = $R1 - $R3

Memory Access Instructions
1001 -- LW, result = Memory[$R3 + offset]
1010 -- SW, Memory[$R3 + offset] = result

Control Flow Instructions
1011 -- beq, Branch to (PC+2) when $R1 = $R2
1100 -- Jump offset Jump to {PC [15:], (offset << 1)}



