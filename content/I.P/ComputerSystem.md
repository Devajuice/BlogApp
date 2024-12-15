+++
date = '2024-12-15T17:11:10+05:30'
draft = false
title = 'Computer System'
description = "A computer system is a complex interplay of hardware and software components that work together to process information."
image = "/images/I.P/CS.webp"
imageBig = "/images/I.P/CS2.webp"
categories = ["Notes", "I.P"]
author = ["Devajuice"]
avatar = "/images/avatar.webp"
+++
# Introduction

- A computer system primarily comprises a central processing unit, memory, input/output devices, and storage devices.

# Central Processing Unit(CPU)

- It is the electronic circuitry of a computer that carries out the actual processing and is usually referred to as the brain of the computer.
- ***CPU*** stores the data as well as instructions in its local memory called ***registers***.
- Arithmetic Logic Unit(***ALU***) and Control Unit(***CU***). ALU performs all the arithmetic and logic operations that need to be done as per the instructions in a program. ***CU*** controls sequential instruction execution, interprets instructions, and guides data flow through the computer's memory. ***CPU*** is also popularly known as a ***microprocessor***.

# Input Devices

- Data entered through the input device is temporarily stored in the main memory(also called ***RAM***) of the computer system.

# Output Devices

- The device that receives data from a computer system for display, physical production, etc, is called an output device. It converts digital information into human understandable form.

# Computer Memory

- A computer system needs memory to store the data and instructions for processing.
- The secondary memory(also called storage device) is used to store data, instructions and results permanently and for future use.

## Units of Memory

- A computer system uses binary numbers to store and process data. The binary digits 0 and 1, which are the basic units of memory, are called bits. Further, these bits are grouped to form words. A 4-bit word is called a **Nibble**. A two-nibble word, an 8-bit word, is called a **Byte**.

|     Unit     |    Description    |     Unit      |  Description   |
| :----------: | :---------------: | :-----------: | :------------: |
| KB(Kilobyte) | 1 KB = 1024 Bytes | PB(Petabyte)  | 1 PB = 1024 TB |
| MB(Megabyte) |  1 MB = 1024 KB   |  EB(Exabyte)  | 1 EB = 1024 PB |
| GB(Gigabyte) |  1 GB = 1024 MB   | ZB(Zettabyte) | 1 ZB = 1024 EB |
| TB(Terabyte) |  1 TB = 1024 GB   | YB(Yottabyte) | 1 YB = 1024 ZB |

# Types of Memory

- Computers have two types of memories namely - **Primary Memory** and **Secondary Memory**.

## Primary Memory

- The primary memory is an essential component of computer system. Program and data are loaded into the ***primary memory*** before processing. The ***CPU*** interacts directly with the ***primary memory*** to perform read/write operation. It is of two types

1. **Random Access Memory(RAM)**
2. **Read Only Memory(ROM)**

- ***RAM*** is ***volatile***, as long as the power is supplied to the computer, it retains the data in it. But as soon as the power supply is turned off, all the contents of **RAM** are **wiped out**. It is used to store data *temporarily* while the computer is working. Whenever the computer is started or a software application is launched, the required program and data are loaded into RAM for processing. **RAM** is usually referred to as **main memory** and **it is faster** than the **secondary memory** or storage device.
- ***ROM*** is ***non-volatile***, means its contents are not lost even when the power is turned off. It is used as a small but faster **permanent storage** for the contents **which are rarely changed**, the startup program(boot loader) that loads the operating system into RAM is stored in a **ROM**.

## Cache Memory

- RAM is faster than secondary storage, but not as fast as a computer processor. So, because of RAM, A CPU may have to slow down. To speed up the operations of the CPU, a very high speed memory is placed between the CPU and the primary memory known as **cache**.

## Secondary Memory

- Primary memory (RAM/ROM) is fast but limited and volatile. Secondary memory (like SSDs) is slower but permanent and cheaper, providing long-term storage for data and instructions.

# Software

- Hardware needs to be operated by a set of instructions. These sets of instructions are referred to as software. It is that component of a computer system, which we cannot touch or view physically. It comprises of the instructions and data to be processed using the computer hardware. The computer software and hardware complete any task together.

## System Software

- The software that provides the basic functionality to operate a computer by interacting directly with its constituent hardware is termed as system software. A system software knows how to operate and use different hardware components of a computer. It provides services directly to the end user, or to some other software.

### Operating System

- As the name implies, operating system is a system software that operates the computer. An operating system is the most basic system software, without which other software cannot work. The operating system manages other application programs and provides access and security to the users of the system.

### System Utilities

- Software used for maintenance and configuration of the computer system is called system utility. Some system utilities are shipped with the operating system, for example *disk defragmentation tool*, *formatting utility*, etc.

# Application Software

- The system software provides the core functionality of the computer system.

## General Purpose Software

- The application software developed for generic applications, to cater to a bigger audience in general are called general purpose software.

## Customised Software

- These are custom or tailor-made application software, that are developed to meet the requirements of a specific organisation or an individual.

# Proprietary or Free and Open Source Software

- Developers of some software allow public to freely use their software along with source code with an aim to improve further with each other’s help. Such software is known as Free and Open Source Software (FOSS).
- When software to be used has to be purchased from the vendor who has the copyright of the software, then it is a proprietary software.
