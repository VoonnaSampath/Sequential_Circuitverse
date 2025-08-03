# 4 Bit Asynchronous Updown Counter – CircuitVerse

## 🧠 Project Overview
This project demonstrates the implementation of a **4-bit Asynchronous Up/Down Counter** using [CircuitVerse](https://circuitverse.org). The counter increments or decrements its binary output based on a control input, simulating ripple carry behavior in sequential digital circuits.

## ✅ Key Features
- **Functionality**: Counts from 0 to 15 (UP) or 15 to 0 (DOWN) asynchronously.
- **Inputs**:
  - `CLK` – Clock signal
  - `Mode` – Control signal (0 for up, 1 for down)
  - `CLR` – Asynchronous clear (reset)
- **Outputs**:
  - `Q0` to `Q3` – 4-bit binary output
- **Controlled using**: Rising edge-triggered flip-flops and `UP/DOWN` mode control

## 📂 Files Included
- `4 Bit Asynchronous Updown Counter.cv` – Raw exported CircuitVerse file
- `4 Bit Asynchronous Updown Counter.png` – Schematic image of the circuit
- `README.md` – This documentation file

## 🔗 Live Simulation
[Click here to view the project on CircuitVerse](https://circuitverse.org/simulator/edit/3-bit-asynchronous-updown-counter)

## 🛠 Tools Used
- [CircuitVerse](https://circuitverse.org) – Open-source digital logic design simulator

---

## 📊 Truth Table (Simplified)

| Count | Q3 | Q2 | Q1 | Q0 |
|-------|----|----|----|----|
| 0     | 0  | 0  | 0  | 0  |
| 1     | 0  | 0  | 0  | 1  |
| ...   | .. | .. | .. | .. |
| 15    | 1  | 1  | 1  | 1  |

> Direction of count depends on the `UP/DOWN` control:
> - UP (`0`): Increments binary output
> - DOWN (`1`): Decrements binary output

---

> 💡 Use this module to understand ripple delay, asynchronous behavior, and mode control in real counters. A key building block in digital system design and VLSI.