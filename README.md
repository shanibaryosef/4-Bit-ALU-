# 4-Bit-ALU-
This project presents the design and implementation of a simplified 4-bit Arithmetic Logic Unit (ALU), developed as part of the Introduction to VLSI course at Tel Aviv University (Winter 2024/5 semester).

The project aims to give hands-on experience in designing, planning, and implementing a digital VLSI circuit, similar to real-world industry processes.
Project Specifications
Inputs:

    A[3:0], B[3:0], C[3:0] – Three 4-bit logical inputs.
    Each input is stored in a register before processing.

Outputs:

    Y[5:0] – A 6-bit output, stored in a register.

Operations:

    All arithmetic operations are performed using two’s complement representation.
    The ALU supports the following operations:
        ADD: ⟨X⟩ = ⟨A⟩ + ⟨B⟩
        SUB: ⟨Y⟩ = ⟨X⟩ - ⟨C⟩
    The design includes an internal register X[4:0] to store the sum of A and B.

Technical Constraints:

    Supply Voltage: Single VDD at 1.2V.
    Area: Total realization area of the adder must not exceed 150% of the sum of all cells' areas.
    Timing: Rise/Fall times (10%-90%) at the inputs must not exceed 50ps.

Design Details

    Adder Architecture: Implemented using a Brent-Kung Adder, determined according to group ID digits.
    Registers: Multiple D Flip-Flops (4-bit, 5-bit, and 6-bit) are used to store inputs, intermediate results, and outputs.
    Subtractor: Implemented using the result of the adder and performing bitwise NOT and addition for subtraction.

Tools & Technologies

    Cadence Virtuoso
    gpdk045/gsclib045 Technology Library
