---
title: "Getting Started"
permalink: /apple2emu/getting-started/
excerpt: ""
date: 2016-07-08
author_profile: true
header:
   overlay_image: programming-header.jpg
---

{% include base_path %}

The starting point for writing the emulator was starting with the CPU.  The
original Apple \]\[ is a 6502 processor.  One of the benfits for this project
for such an old processor is that the instruction set is small (< 256 opcodes).
The small number of opcodes makes creating the code relatively easy.  

Before getting into detail about writing the CPU emulation layer, it will 
be beneficial to talk about architecture, both of the code and of the machine
that we are emulating.  I also had to make some decisions on exactly what
I would emulate and to what degree I would try to achieve "perfect" as
opposed to "good enough".  For example, we need perfect emulation of the CPU
layer because the opcodes just need to work.  For emulating video, we might
not need to be exactly perfect.  

## Von Neumann Model
The Von Neumann architecture model describes the design of a computer which
contains:

* Central Processing Unit
   * Arithmetic Unit
   * Control Unit
* Memory

The following diagram shows the basic design of such a machine:

![](/images/von_neumann.png)

Note that in the diagram, there are also input and output devices.  Input
devices can be considered to be hardware such as a keyboard, and the output
devices are items like the monitor (or video display device).  So when working
on the emulator, the main parts shown in the above diagram are the areas that
need to be emulated.  

The following outlines the major systems and the major ideas to consider when
writing an emulator for that layer

## Memory

## CPU

## Input

## Ouput
