# MOD-5 Synchronous Up Counter – CircuitVerse

## 🧠 Project Overview
This project demonstrates the implementation of a **MOD-5 Synchronous Up Counter** using [CircuitVerse](https://circuitverse.org). Unlike asynchronous counters, all flip-flops in this design are triggered simultaneously on the same clock edge, making it faster and more reliable for higher-frequency applications. The counter cycles through binary states from 0 to 4 and resets to 0 after reaching 5.

## ✅ Key Features
- **Functionality**: Counts synchronously from 0 to 4 (mod-5) and resets on 5
- **Inputs**:
  - `CLK` – Common clock input to all flip-flops
  - `CLR` – (Optional) Reset input to force the count to 0
- **Outputs**:
  - `Q2`, `Q1`, `Q0` – 3-bit binary output representing the current count
- **Controlled using**: Logic to detect count of 5 and reset all outputs to 0

## 📂 Files Included
- `MOD 5 synchronous Up Counter.cv` – Raw exported CircuitVerse file
- `MOD 5 synchronous Up Counter.png` – Schematic image of the MOD-5 counter
- `README.md` – This documentation file

## 🔗 Live Simulation
[Click here to view the project on CircuitVerse](https://circuitverse.org/simulator/edit/mod-5-synchronous-up-counter-using-t-ff)

## 🛠 Tools Used
- [CircuitVerse](https://circuitverse.org) – Open-source digital logic design simulator

---

## 📊 MOD-5 Counter Truth Table

| CLK Pulse | Q2 | Q1 | Q0 | Decimal |
|-----------|----|----|----|---------|
| 0         | 0  | 0  | 0  | 0       |
| 1         | 0  | 0  | 1  | 1       |
| 2         | 0  | 1  | 0  | 2       |
| 3         | 0  | 1  | 1  | 3       |
| 4         | 1  | 0  | 0  | 4       |
| 5         | 0  | 0  | 0  | 0 (Reset) |

> The circuit resets once it detects the count "5" (binary 101), ensuring a MOD-5 behavior.

---

> 💡 This type of counter is useful in applications requiring precise count limits, such as digital clocks, frequency dividers, and control timing logic in VLSI circuits.