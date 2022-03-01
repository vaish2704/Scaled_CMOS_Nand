
# Scaled 2-Input CMOS Nand Gate using 28nm PDK

Here we have designed a Scaled-2 Input CMOS NAND Gate using the 28nm Process Design Kit available on Synopsys Custom Compiler and analyzed the output and delay in comparison to a Conventional CMOS NAND Gate using the PrimeWave Design Environment.

# Abstract

Nowadays, we observe that a complementary-metaloxide-semiconductor (CMOS) is widely used in large scale integrated circuits. Here we aim to design a scaled 2-input CMOS NAND Gate on a 28nm scale and analyze its output behavior along with the delay analysis for the same in comparison to a conventional 2-input CMOS NAND Gate. NAND gates are basic universal gates because with the help of these gates, we can create any digital circuit. Most of the CMOS Nand gate design techniques need either a p-logic block or an n-logic block for evaluation of input and output behavior at a transistor level.

# Contents

# Introduction

In the world of Digital Circuits, NAND gates are one of the most prominent logic gates which produce a low output only when all of the inputs are high(i.e. logic 1).The output of these gates is simply the invert/complement of an AND gate.They are one of the two Universal gates(the other being NOR gates) but are more common in the industry than the latter, the reason for this being the Design Implementation easeness and the less complex approach of minterms involved in NAND Gate logic. The recent changes in the VLSI Industry in view of the shrinking size of transistors has changed the way these devices impact the world. The CMOS NAND Gates are widely used in a lot of digital, analog and mixed signal circuits.
In CMOS technology, both N-type and P-type transistors are used to design logic functions. The same signal which turns ON a transistor of one type is used to turn OFF a transistor of the other type. This characteristic is the root reason allowing us to design our Conventional and Scaled NAND logic.
The work that was done using the 28nm Library file in this design is divided into three sections-
1) Design of Conventional NAND gate
2) Design of Scaled NAND gate
3) Delay comparison

# Conventional NAND Gate
## Reference Circuit
<p align="center">
<img src="Reference_Ckts_Waveform/Ref_Ckt_Conv.jpg"></br>
Fig: Reference Circuit of Conventional NAND Gate 
</p>

## Design Explanation
### Truth Table
<p align="center">
<img src="Reference_Ckts_Waveform/NAND-TT.png"></br>
Fig: Truth Table of NAND Gate 
</p>

Case 1: When A=0, B=0
As VA and VB both are low, both the pMOS will be ON and both the nMOS will be OFF. So the output Vout will get two paths through two ON pMOS to get connected with Vdd. The output will be charged to the Vdd level. The output line will not get any path to the GND as both the nMOS are off. So, there is no path through which the output line can discharge. The output line will maintain the voltage level at Vdd, hence Vout will be high. 

Case 2: When A=0, B=1
pMOS1 and pMOS2 are in parallel. Though pMOS2 is OFF, still the output line will get a path through pMOS1 to get connected with Vdd. nMOS1 and nMOS2 are in series. As nMOS1 is OFF, so Vout will not be able to find a path to GND to get discharged. This in turn results the Vout to be maintained at the level of Vdd, hence Vout will be high.

Case 3: When A=1, B=0
Works in a similar fashion as in case 2, hence Vout will be high.

Case 4: When A=1, B=1
In this case, both the pMOS are OFF. So, Vout will not find any path to get connected with Vdd. As both the nMOS are ON, the series connected nMOS will create a path from Vout to GND. Since, the path to ground is established, Vout will be discharged, hence low.

## Reference Waveform
<p align="center">
<img src="Reference_Ckts_Waveform/Ref_Op_Conv.jpg"></br>
Fig: Reference Waveform of Conventional NAND Gate 
</p>



# Conventional NAND Gate
## Reference Circuit

## Circuit Working Principle

## Reference Circuit
