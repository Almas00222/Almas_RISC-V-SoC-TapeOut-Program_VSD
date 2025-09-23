# Day 1: Basics of Verilog RTL Design & Synthesis

Welcome to **Day 1** of the RTL Workshop!  
This session introduces you to digital design using Verilog, open-source simulation with **Icarus Verilog (iverilog)**, and logic synthesis with **Yosys**. Through labs and explanations, you’ll build a solid starting point for RTL design.

---

## Table of Contents

1. [Simulator, Design, and Testbench Explained](#1-simulator-design-and-testbench-explained)  
2. [Getting Started with iverilog](#2-getting-started-with-iverilog)  
3. [Hands-on Lab: 2-to-1 Multiplexer Simulation](#3-hands-on-lab-2-to-1-multiplexer-simulation)  
4. [Code Walkthrough](#4-code-walkthrough)  
5. [Intro to Yosys & Gate Libraries](#5-intro-to-yosys--gate-libraries)  
6. [Synthesis with Yosys](#6-synthesis-with-yosys)  
7. [Recap](#7-recap)

---

## 1. Simulator, Design, and Testbench Explained

### Simulator
A **simulator** verifies your digital design by applying inputs and observing outputs before moving to hardware.

### Design
The **design** is your Verilog description of the desired logic.

### Testbench
A **testbench** provides stimulus (inputs) to the design and checks if the outputs behave as expected.

<div align="center">
  <img src="https://github.com/user-attachments/assets/93927b96-df80-4da5-b801-284fc2cc6757" alt="Design & Testbench Overview" width="70%">
</div>

---

## 2. Getting Started with iverilog

**iverilog** is an open-source tool for Verilog simulation. The general flow is:

<div align="center">
  <img src="https://github.com/user-attachments/assets/3ca190fb-cfa4-4abb-b9e1-0151b3c4bdba" alt="iverilog Simulation Flow" width="70%">
</div>

- Provide the design and testbench to iverilog.  
- Simulation creates a `.vcd` file for waveform viewing in GTKWave.

---

## 3. Hands-on Lab: 2-to-1 Multiplexer Simulation

We’ll simulate a **2-to-1 multiplexer** using iverilog.

### Step 1: Clone Repository
```bash
git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git
cd sky130RTLDesignAndSynthesisWorkshop/verilog_files
