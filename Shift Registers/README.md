# Shift Registers Collection – CircuitVerse

## 🧠 Project Overview
This project showcases the implementation of **six types of shift registers** using [CircuitVerse](https://circuitverse.org). All designs are bundled into a single `.cv` file, with individual circuits for:
- **SISO** (Serial-In Serial-Out)
- **SIPO** (Serial-In Parallel-Out)
- **PIPO** (Parallel-In Parallel-Out)
- **PISO** (Parallel-In Serial-Out)
- **Bidirectional Register**
- **Universal Shift Register**

These circuits illustrate fundamental data storage and transfer operations crucial to sequential digital systems and VLSI design.

---

## ✅ Key Features

- **Functionality**:
  - Serial and parallel data shift mechanisms
  - Directional and mode-controlled registers
- **Inputs**:
  - CLK – Common clock input
  - D / P[0–3] – Data inputs (serial or parallel)
  - Mode / DIR – Mode select and direction controls (for advanced registers)
- **Outputs**:
  - Q[0–3] – Output bits (serial or parallel depending on type)
- **Controlled Using**:
  - Flip-flop chains, multiplexers, and control logic

---

## 📊 Register Functionality Overview

| Register Type | Description |
|---------------|-------------|
| **SISO**      | Serial input is shifted through all flip-flops to serial output |
| **SIPO**      | Serial input is shifted into flip-flops and read out in parallel |
| **PIPO**      | All bits loaded and read simultaneously (parallel) |
| **PISO**      | Parallel data loaded and shifted out serially |
| **Bidirectional** | Shifts data left or right based on control signal |
| **Universal** | Supports all four modes: SISO, SIPO, PISO, PIPO via mode control |

---

## 📂 Files Included

| File | Description |
|------|-------------|
| `Shift Registers.cv` | Raw exported CircuitVerse file with all six registers |
| `SISO.png` | Schematic image of Serial-In Serial-Out register |
| `SIPO.png` | Schematic of Serial-In Parallel-Out register |
| `PIPO.png` | Schematic of Parallel-In Parallel-Out register |
| `PISO.png` | Schematic of Parallel-In Serial-Out register |
| `Bidirectional.png` | Bidirectional shift register schematic |
| `Universal.png` | Universal shift register with mode control |
| `README.md` | Documentation for this project |

---

## 🔗 Live Simulation
[Click here to view the complete project on CircuitVerse](https://circuitverse.org/simulator/edit/registers-6666eda0-88ac-4052-85df-644bfa2366dd)

---

## 🛠 Tools Used

- [CircuitVerse](https://circuitverse.org) – Open-source digital circuit simulator

---

> 💡 These designs are essential for understanding data flow mechanisms in memory blocks, processors, and VLSI subsystems. You can use this repo to showcase digital design proficiency in interviews and portfolios.