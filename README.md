
RISC-V 5-Stage Pipelined Processor
Overview
This project implements a 5-stage RISC-V pipelined processor with support for various instruction types, including R, I, U, J, B, and S types. The processor also includes support for Control and Status Registers (CSR), as well as interrupt and exception handling.

Architecture
The processor is designed with the following five stages:

Instruction Fetch (IF):

Responsible for fetching instructions from memory.
Retrieves the instruction pointed to by the program counter.
Instruction Decode (ID):

Decodes the fetched instruction to identify the operation and operand addresses.
Determines the type of instruction (R, I, U, J, B, S).
Execute (EX):

Performs the actual computation or operation specified by the instruction.
Handles ALU operations and branching.
Memory (MEM):

Manages data memory access.
Performs load and store operations.
Writeback (WB):

Writes the result of the instruction back to registers.
Handles updates to control and status registers.
Supported Instruction Types
The processor supports the following RISC-V instruction types:

R-Type Instructions: Arithmetic and logic instructions with three register operands.

I-Type Instructions: Immediate instructions with an immediate value and a register operand.

U-Type Instructions: Unconditional jump instructions with a 20-bit immediate value.

J-Type Instructions: Jump instructions with a 20-bit immediate value for jumps and branches.

B-Type Instructions: Branch instructions with a 12-bit immediate value for conditional branches.

S-Type Instructions: Store instructions with a base register, destination register, and a 12-bit immediate value.

CSR Support
The processor includes support for Control and Status Registers (CSR) for managing system control and status. It allows privileged instructions to access and modify CSR values.

Interrupt and Exception Handling
The processor implements interrupt and exception handling mechanisms to gracefully handle unexpected events or requests. It includes mechanisms for handling external interrupts and exceptions raised during the execution of instructions
