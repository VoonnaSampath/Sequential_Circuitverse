# Flipflops Using MUX  – CircuitVerse

## 🧠 Project Overview
This project demonstrates the implementation of **basic flip-flops (SR, D, JK, and T)** using only **multiplexers (MUX)** instead of traditional gates or latch structures. The design uses **combinational logic behavior of MUX** to simulate the next-state logic of each flip-flop. This approach showcases how sequential circuits can be modeled from purely combinational components.

## ✅ Key Features

- **Functionality**:
  - **SR Flip-Flop**: Set-Reset bistable latch with invalid state handling
  - **D Flip-Flop**: Single-data input storage
  - **JK Flip-Flop**: Edge-sensitive toggle device
  - **T Flip-Flop**: Toggle flip-flop (used in counters)
- **Inputs**:
  - `S`, `R`, `D`, `J`, `K`, `T` – Depending on flip-flop type
  - `CLK` – Clock signal
  - `Q_prev` – Feedback to emulate state (held in latch or loop)
- **Outputs**:
  - `Q` – Main output
  - `Q'` – Complement output
- **Controlled using**: Only MUX logic; no NAND/NOR gates

## 📂 Files Included

- `Flipflops Using MUX.cv` – Complete CircuitVerse file with all flip-flops
- `SR FF using 2X1 mux.png` – Schematic for SR flip-flop using MUX
- `D FF using 2X1 mux.png` – Schematic for D flip-flop using MUX
- `JK using 2X1 mux.png` – Schematic for JK flip-flop using MUX
- `T FF using 2X1 mux.png` – Schematic for T flip-flop using MUX
- `README.md` – Documentation for this module

## 🔗 Live Simulation

[Click here to view the project on CircuitVerse](https://circuitverse.org/simulator/edit/flipflops-using-mux)

## 🛠 Tools Used

- [CircuitVerse](https://circuitverse.org) – For schematic design and simulation

---

## ⚙️ Flip-Flop Logic Using MUX

### 1️⃣ SR Flip-Flop using MUX

- Logic: Q_next = (S == 1) ? 1 :(R == 1) ? 0 : Q_prev;
- Truth Table:

| S | R | Q(t+1) |
|---|---|--------|
| 0 | 0 |  Q     |
| 0 | 1 |  0     |
| 1 | 0 |  1     |
| 1 | 1 |  Invalid |

---

### 2️⃣ D Flip-Flop using MUX

- Logic: Q_next = D
- Truth Table:

| D | CLK ↑ | Q(t+1) |
|---|--------|--------|
| 0 |   ↑    |   0    |
| 1 |   ↑    |   1    |

- Implemented using one MUX to route D to Q when clock triggers.

---

### 3️⃣ JK Flip-Flop using MUX

- Logic: Q_next = (J == 0 && K == 0) ? Q_prev :(J == 0 && K == 1) ? 0 :(J == 1 && K == 0) ? 1 : ~Q_prev;
- Truth Table:

| J | K | Q(t+1) |
|---|---|--------|
| 0 | 0 |   Q    |
| 0 | 1 |   0    |
| 1 | 0 |   1    |
| 1 | 1 |  ~Q    |

---

### 4️⃣ T Flip-Flop using MUX

- Logic:Q_next = (T == 1) ? ~Q_prev : Q_prev;
- Truth Table:

| T | CLK ↑ | Q(t+1) |
|---|--------|--------|
| 0 |   ↑    |   Q    |
| 1 |   ↑    |  ~Q    |

---

## 🔁 Why Use MUX for Flip-Flops?

- Simulates **next state logic** using controlled data paths
- Helps in **testable and reduced gate-count designs**
- Encourages understanding of **functional decomposition** of sequential circuits

---

> 💡 This MUX-only flip-flop collection offers an unconventional but educational approach to building sequential memory elements — suitable for datapath control, digital system modeling, and FSMs in VLSI design.