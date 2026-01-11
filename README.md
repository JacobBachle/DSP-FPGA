# DSP on FPGA – Cyclone V (DE0-CV)

This repository contains collaborative research and development work focused on
digital signal processing (DSP) implementations on FPGA hardware.

The primary focus is on **numeric formats, quantization effects, and architectural
trade-offs** in FPGA-based DSP systems using the Terasic DE0-CV (Cyclone V) platform.

---

## Hardware Platform
- Terasic DE0-CV FPGA Development Board
- Intel (Altera) Cyclone V E – 5CEBA4F23C7N

---

## Primary Project
**FFT Butterfly Processor Numeric Format Comparison**
- 16-bit floating-point implementation
- 16-bit Posit number format implementation
- Quantization error and resource usage comparison

Reference designs are based on:
*Digital Signal Processing with Field Programmable Gate Arrays (4th Edition)*
by Uwe Meyer-Baese.

---

## Repository Structure
docs/ Project documentation and learning resources
rtl/ VHDL source files
tb/ Testbenches
scripts/ Python / MATLAB analysis scripts
results/ Plots, tables, and reports

---

## Documentation
- Project overview: `docs/project-overview.md`
- Learning resources: `docs/learning-resources.md`
- Documentation standard: `docs/documentation-standard.md`
- Contributing guidelines: `CONTRIBUTING.md`

---

## Status
Early-stage research and development.
