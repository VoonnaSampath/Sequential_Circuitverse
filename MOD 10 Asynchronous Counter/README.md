# MOD-10 Asynchronous Counter – CircuitVerse

## 🧠 Project Overview
This project demonstrates the implementation of a **MOD-10 Asynchronous Counter** (also known as a decade counter) using [CircuitVerse](https://circuitverse.org). It counts from 0 to 9 in binary and resets automatically to 0 after reaching 9, using asynchronous ripple counter logic.

## ✅ Key Features
- **Functionality**: Counts binary values from 0 to 9 (i.e., MOD-10)
- **Inputs**:
  - `CLK` – Clock pulse input
  - `CLR` – Asynchronous clear signal to reset the count
- **Outputs**:
  - `Q0` to `Q3` – 4-bit binary output representing the count
- **Controlled using**: Flip-flop chain with logic to reset after 1001 (decimal 9)

## 📂 Files Included
- `mod10_counter.cv` – Raw exported CircuitVerse file
- `mod10_counter.png` – Schematic image of the circuit
- `simulation.mp4` – (Optional) Working simulation video
- `README.md` – Documentation for this module

## 🔗 Live Simulation
[Click here to view the project on CircuitVerse](https://circuitverse.org/simulator/edit/mod-10-asynchronous-counter-c08dbcd4-8c44-4f98-94f9-21f7bd925544)

## 🛠 Tools Used
- [CircuitVerse](https://circuitverse.org) – Open-source digital circuit simulator

---

## 📊 MOD-10 Counter Truth Table

| Decimal | Q3 | Q2 | Q1 | Q0 |
|---------|----|----|----|----|
| 0       | 0  | 0  | 0  | 0  |
| 1       | 0  | 0  | 0  | 1  |
| 2       | 0  | 0  | 1  | 0  |
| 3       | 0  | 0  | 1  | 1  |
| 4       | 0  | 1  | 0  | 0  |
| 5       | 0  | 1  | 0  | 1  |
| 6       | 0  | 1  | 1  | 0  |
| 7       | 0  | 1  | 1  | 1  |
| 8       | 1  | 0  | 0  | 0  |
| 9       | 1  | 0  | 0  | 1  |
| Reset   | 0  | 0  | 0  | 0  |

> The counter resets to 0000 after reaching 1001 (decimal 9) using asynchronous clear logic.

---