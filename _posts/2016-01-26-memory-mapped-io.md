---
layout: post
title: memory mapped I/O
publish: true
---

# Memory mapped I/O Devices and how they work

This text explains how 2 I/O devices, precisely the screen and keyboard,
work. The technique explained here is a memory mapped technique.

Memory is systematically or categorically divided. Memory addresses start from
0 to n-1.

An n-bit computer often has n registers with register addresses starting from
R0 to R(n-1). Well, in most cases, these registers reside on the CPU chip in
order to speed up data access.

The physical device called RAM or memory is virtualized into one big 1
dimensional array, where the addresses of this array range from 0 - n-1, where
n is the number of bits of this machine. Each of the array cells has a capacity
of n bits.

With that said, systems use certain symbols to name the various categories of
memory units and registers.

The first n-1 memory addresses refer to registers: R1 - R(n-1)

Then comes predefined pointers, some of which point to the above mentioned
registers:

SP, LCL, ARG, THIS, THAT which refer to RAM addresses 0 - 4. Therefore, R2 also
refers to ARG.


And then comes our I/O pointers. The symbols SCREEN and KBD are predefined
addresses like 16384(0x4000) and 24576 (0x6000). These addresses are the
addresses of the screen and keyboard memory maps.

## I/O Handling
Let the computer be connected to 2 I/O devices: screen and keyboard. These
devices will interact with our computing platform through the memory maps
specified above or similarly specified.

This implies that drawing pixels on the screen is as simple or as direct as
writing binary values to the memory address or segment associated with the
screen.

Similarly, listening to the keyboard is as direct as listening to the memory
location or segment associated with the keyboard.

The physical IO devices and their memory maps are synchronized via continuous
refresh loops.


### References

Noam Nisan and Shimon Shocken, Elements of Computing Systems
