# Sequential Digital Circuits in CircuitVerse

This repository contains a collection of **sequential digital circuits** implemented and documented in [CircuitVerse](https://circuitverse.org/). Sequential circuits are foundational building blocks in digital electronics, where the output depends not only on the current inputs but also on the history of inputs (i.e., they have memory).

---

## ✅ Included Circuits

Below is a list of typical sequential circuits included in this repository. Each circuit is organized in its own folder.

### 1. D,JK, T Flip-Flop

#### JK Flip-Flop

- **Function:** Versatile flip-flop that eliminates the invalid state of SR Latch; can toggle, set, or reset.

#### D Flip-Flop

- **Function:** Data (Delay) flip-flop that captures input data on a clock edge and stores it until the next clock.

#### T Flip-Flop

- **Function:** Toggle flip-flop; output changes state on each clock pulse if T input is high.

- **Folder:** `D,JK,T Flip-Flop`

### 2. 4-bit Synchronous Counter

- **Function:** Counts from 0 to 15 in binary, incrementing on each clock pulse; all flip-flops share the clock.
- **Folder:** `4-bit-Synchronous-Counter`

### 3. Shift Register

- **Function:** Stores and shifts data serially or in parallel, useful for data transfer and manipulation.
- **Folder:** `Shift-Register`

### 4. 3-bit Synchronous Counter

- Function: Counts from 0 to 7 synchronously with the clock signal.
- Folder: `3-bit-Synchronous-Counter`

### 5. Finite State Machines

- Function: Represents systems that transition between states based on input; used in control logic and sequence detectors.
- Folder: `Finite-State-Machines`

### 6. Flip-Flops Using MUX

- Function: Implements flip-flop behavior using multiplexers to demonstrate internal design logic.
- Folder: `FlipFlops-Using-MUX`

### 7. MOD-5 Synchronous Up Counter

- Function: Counts from 0 to 4 synchronously, then wraps around to 0.
- Folder: `MOD5-Synchronous-UpCounter`

### 8. MOD-10 Asynchronous Counter

- Function: Ripple counter that counts from 0 to 9 asynchronously.
- Folder: `MOD10-Asynchronous-Counter`

---

## 📂 Folder Contents

Each circuit folder typically contains:

- `circuit.cv` — CircuitVerse project file for import and simulation.
- `circuit.png` — Image of the circuit schematic for quick reference.
- `README.md` — Brief documentation about the specific circuit, its operation, and usage.

---

## 🧭 How to Use These Files

To experiment with or modify these circuits:

1. **Download the `.cv` file** from the desired circuit's folder.
2. **Go to [CircuitVerse.org](https://circuitverse.org/)** and log in (or sign up).
3. Click on **"Import Project"** in your dashboard.
4. **Upload the `.cv` file** and import it.
5. Open the imported project to simulate, analyze, or edit the circuit.

You can also view the `circuit.png` image for a quick overview of the circuit's structure.

---

## 🛠 Tools Used

- [CircuitVerse](https://circuitverse.org/) — Design, simulation, and export of digital circuits.

---

Sequential circuits are essential for building memory, counters, registers, and control logic in digital systems, making them crucial for both learning and practical digital design.
