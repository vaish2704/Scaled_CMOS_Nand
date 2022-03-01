
# Scaled 2-Input CMOS Nand Gate using 28nm PDK

Here we have designed a Scaled-2 Input CMOS NAND Gate using the 28nm Process Design Kit available on Synopsys Custom Compiler and analyzed the output and delay in comparison to a Conventional CMOS NAND Gate using the PrimeWave Design Environment.

# Abstract

Nowadays, we observe that a complementary-metaloxide-semiconductor (CMOS) is widely used in large scale integrated circuits. Here we aim to design a scaled 2-input CMOS NAND Gate on a 28nm scale and analyze its output behavior along with the delay analysis for the same in comparison to a conventional 2-input CMOS NAND Gate. NAND gates are basic universal gates because with the help of these gates, we can create any digital circuit. Most of the CMOS Nand gate design techniques need either a p-logic block or an n-logic block for evaluation of input and output behavior at a transistor level.

# Contents

# Introduction

In the world of Digital Circuits, NAND gates are one of the most prominent logic gates which produce a low output only when all of the inputs are high(i.e. logic 1).The output of these gates is simply the invert/complement of an AND gate.They are one of the two Universal gates(the other being NOR gates) but are more common in the industry than the latter, the reason for this being the Design Implementation easeness and the less complex approach of minterms involved in NAND Gate logic. The recent changes in the VLSI Industry in view of the shrinking size of transistors has changed the way these devices impact the world. The CMOS NAND Gates are widely used in a lot of digital, analog and mixed signal circuits.
In CMOS technology, both N-type and P-type transistors are used to design logic functions. The same signal which turns ON a transistor of one type is used to turn OFF a transistor of the other type. This characteristic is the root reason allowing us to design our Conventional and Scaled NAND logic. 
