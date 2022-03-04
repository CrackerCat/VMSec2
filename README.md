# VMSec2
Obfuscation method using virtual machine. Continuation of VMPROTECT

<img src="https://repository-images.githubusercontent.com/236199786/eab7cc00-05b7-11eb-9f91-6ea165c2cc2c" height="200">

<i>A code obfuscation method using virtual machines to protect programs</i>

<a href="https://github.com/eaglx/VMSec2/stargazers"><img src="https://img.shields.io/github/stars/eaglx/VMSec2" alt="Stars Badge"/></a>
<a href="https://github.com/eaglx/VMSec2/network/members"><img src="https://img.shields.io/github/forks/eaglx/VMSec2" alt="Forks Badge"/></a>
<a href="https://github.com/eaglx/VMSec2/blob/master/LICENSE"><img src="https://img.shields.io/github/license/eaglx/VMSec2?color=2b9348" alt="License Badge"/></a>
[![GitHub release](https://img.shields.io/github/release/eaglx/VMSec2)](https://GitHub.com/eaglx/VMSec2/releases/)
![Progress](https://progress-bar.dev/1/?title=progress-v0.1)

VMSec2 is a virtual machine that simulates a CPU along with a few other hardware components. It allows to perform arithmetic operations, reads and writes to memory and interacts with I/O devices. It can only understand a machine language which is designated for this vm. Virtual machines used in code obfuscation are completely different than common virtual machnines. They are very specific to the task of executing a few set of instructions. Each instruction is given a custom opcode (often generated at random).

:warning: Tested only on Linux!

:recycle: Continuation of [VMPROTECT](https://github.com/eaglx/VMPROTECT).

## Table of contents
* [Requirements](#requirements)
* [Compiler](#compiler)
* [Disclaimer](#disclaimer)

## Requirements
* NASM [tested on 2.13.02]
* Python3 [tested on 3.6.9]
* Tkinter [tested on 8.6]
* g++ [tested on 7.5.0]
* make [tested on 4.1]

## Compiler
The *nasm* as compiler is used for compilation a code. Remember to include the *vm.inc* file with definitions of opcodes in your programs. An example program for virtual machine is shown below.

```nasm
%include "vm.inc"   ; Or full path to this file!

start:

```
