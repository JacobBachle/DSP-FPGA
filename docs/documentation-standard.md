# Documentation Standard

This document defines the required standard for documentation and learning
resource contributions to this repository.

Compliance with this standard is **mandatory** for all contributors.

---

## Learning Resource Entries

For learning resources, every contribution must include **all** of the following:

1. A **hyperlink or reference** to the resource  
   - Listed under either **Cited Resources** or **Created Resources**
2. A **brief description** of the resource
3. A **brief justification** explaining *why the resource was included*

---

## Formatting Requirements

- The **description** and **reason for inclusion** must be highlighted using a
  **contributor-specific color**.
- Each contributor is assigned a **unique color** upon approval.
- Contributors must use their assigned color **consistently** across all entries.
- Contributors may not use another contributor’s color.

Color highlighting is used to:
- Attribute contributions clearly
- Improve readability during review
- Maintain accountability in collaborative documentation

---

## Example Entry

```md
https://example.com/resource-link  
<span style="color:#1f77b4">Description:</span> Short description of the resource.  
<span style="color:#1f77b4">Reason:</span> Explanation of why this resource is relevant.

---

# 📄 `docs/project-overview.md`

```md
# Project Overview

This document provides a high-level overview of the DSP-on-FPGA collaboration,
including hardware context, project goals, and planned work.

---

## Purpose

The goal of this project is to explore and evaluate digital signal processing
architectures implemented on FPGA hardware, with a specific focus on how
different numeric formats impact accuracy, resource usage, and performance.

---

## Hardware Platform

### Development Board
- Terasic DE0-CV FPGA Development Board

### FPGA Device
- Intel (Altera) Cyclone V E
- Device: 5CEBA4F23C7N

---

## Reference Material

This project is primarily based on examples and methodologies from:

- *Digital Signal Processing with Field Programmable Gate Arrays (4th Edition)*
  by Uwe Meyer-Baese

Companion code repository:
https://github.com/uwemeyerbaese/DSP_with_FPGAs_ed4

---

## Project Proposals

### Project A – FFT Numeric Format Comparison (Primary)

Implement and evaluate an FFT butterfly processor using different numeric formats.

Scope:
- Study `FFT256.vhd` reference design
- Implement butterfly processor using:
  - 16-bit floating-point
  - 16-bit Posit number format
- Compare implementations using:
  - Quantization error metrics
  - Resource utilization (LUTs, DSPs, registers)
  - Numerical stability across test signals

---

### Project B – Multi-Channel ICA Extension (Backup)

Extend an existing two-channel ICA (Independent Component Analysis) system to
support a third signal channel.

This project is retained as a secondary or fallback option.

---

## Planned Tooling

- Intel Quartus Prime (Lite / Standard)
- ModelSim / Questa for VHDL simulation
- Python / MATLAB for test-vector generation and analysis
- Git and GitHub for version control

---

## Next Steps

1. Study baseline `FFT256.vhd` implementation
2. Identify and isolate butterfly processing blocks
3. Define numeric formats (FP16 vs Posit16)
4. Create simulation testbench and golden reference
5. Evaluate quantization error and FPGA resource usage

This document will evolve as the project progresses.
