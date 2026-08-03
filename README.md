# Half Subtractor using Verilog

## Overview
A Half Subtractor is a combinational logic circuit that subtracts two single-bit binary numbers. It has two inputs:

- A (Minuend)
- B (Subtrahend)

and two outputs:

- Difference (D)
- Borrow (Bo)

## Truth Table

| A | B | Difference (D) | Borrow (Bo) |
|---|---|----------------|-------------|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 |

## Boolean Expressions

Difference = A XOR B

Borrow = A' AND B

## Circuit Diagram

Difference = A ⊕ B

Borrow = A̅ · B

## Files

- `half_subtractor.v` - Verilog design
- `half_subtractor_tb.v` - Testbench
- `simulation_results.png` - Simulation waveform
- `README.md` - Documentation

## Simulation Tool

- ModelSim
- Vivado
- Icarus Verilog
- GTKWave

## Expected Output

```
A=0 B=0 Difference=0 Borrow=0
A=0 B=1 Difference=1 Borrow=1
A=1 B=0 Difference=1 Borrow=0
A=1 B=1 Difference=0 Borrow=0
```

## Author

Your Name