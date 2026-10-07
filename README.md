# Microkernel IPC and Isolation

A systems project exploring performance, isolation, and inter-process communication (IPC) in microkernel-based operating systems, with a focus on seL4, ChCore, and the UnderBridge approach.

## Overview

Microkernels provide strong isolation by keeping the kernel small and moving system services into separate components. However, communication between these components can introduce additional IPC overhead.

This project studies the trade-off between isolation and communication performance in microkernel systems and explores the UnderBridge approach for improving intra-kernel communication while maintaining isolation.

## Objectives

- Study microkernel architecture and system isolation
- Understand inter-process communication (IPC) mechanisms
- Explore the UnderBridge approach for reducing IPC overhead
- Work with the ChCore microkernel
- Build and execute the system using QEMU
- Examine performance across different microkernel configurations

## Implementation

The project includes hands-on work with the ChCore microkernel environment and its build and execution workflow.

The experimental environment uses:

- Linux
- ChCore
- seL4-related tooling
- QEMU
- Docker
- C/C++
- CMake
- GDB

The provided Python script also automates the execution of a seL4 environment on VMware by managing virtual machines, mounting a virtual disk, copying kernel and initialization images, and collecting VM console output.

## Evaluation

The study examines IPC performance and isolation mechanisms across microkernel systems including:

- seL4
- Google Zircon
- Fiasco.OC
- ChCore
- UnderBridge
- SkyBridge

The evaluation also considers system-level workloads including SQLite, YCSB, and an HTTP server.

## Key Concepts

- Microkernel architecture
- Inter-process communication (IPC)
- Kernel/User isolation
- Memory protection
- Intel Protection Keys (PKU)
- Virtualization
- QEMU
- VMware
- ChCore
- seL4
- System performance evaluation

## Project Structure

```text
microkernel-ipc-isolation/
│
├── seL4vmw.py
├── report.pdf
└── README.md
