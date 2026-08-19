# Half Subtractor using Verilog

## Overview

This project implements a Half Subtractor using Verilog HDL.

A Half Subtractor is a combinational circuit that subtracts two 1-bit binary inputs and produces two outputs: Difference and Borrow.

## Inputs

- `A` – Minuend input
- `B` – Subtrahend input

## Outputs

- `Difference` – Difference between A and B
- `Borrow` – Borrow generated during subtraction

## Logic Equations

Difference = A XOR B

Borrow = A' AND B

## Truth Table

| A | B | Difference | Borrow |
|---|---|------------|--------|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 |

## Files

- `half_subtractor.v` – Verilog design
- `half_subtractor_tb.v` – Testbench
- `README.md` – Project documentation
- `simulation_result.png` – Simulation waveform

## Software Used

- Icarus Verilog
- ModelSim / Vivado
- GTKWave

## How to Run

### Compile

```bash
iverilog -o half_subtractor half_subtractor.v half_subtractor_tb.v