# "1001" Mealy Sequence Detector with 1-bit Overlap – CircuitVerse

## 🧠 Project Overview
This project implements a **Mealy-type finite state machine (FSM)** to detect the sequence **"1001"** in a serial input stream. The design uses **JK flip-flops** for state memory and allows **1-bit overlapping**, meaning it can detect overlapping occurrences of the pattern. Built and simulated using [CircuitVerse](https://circuitverse.org), this FSM is suitable for real-time stream pattern detection applications.

## ✅ Key Features
- **Functionality**: Detects the binary sequence `"1001"` using a Mealy FSM model
- **Design Type**: Mealy machine with 1-bit overlap
- **Flip-Flops Used**: JK Flip-Flops for state memory
- **Inputs**:
  - `X` – Serial input stream (1-bit)
  - `CLK` – Clock signal for synchronization
- **Outputs**:
  - `Z` – Output signal that goes HIGH (1) when the sequence is detected

## 📂 Files Included
- `1001 Sequence Detector (Mealy Machine).cv` – Raw exported CircuitVerse file
- `1001 Sequence Detector (Mealy Machine).png` – Schematic image of the sequence detector
- `1001 Sequence Detector (Mealy Machine) Waveform.png` – Waveform image of the sequence detector
- `README.md` – Documentation for this module

## 🔗 Live Simulation
[Click here to view the project on CircuitVerse](https://circuitverse.org/simulator/edit/1001-sequence-detector-mealy-machine)

## 🛠 Tools Used
- [CircuitVerse](https://circuitverse.org) – Open-source digital circuit simulator

---

## 🧩 How the Mealy Sequence Detector Works

The Mealy machine outputs `Z = 1` **immediately** when the final input bit of the sequence is received, based on both the current **state** and **input**.

### 📐 FSM State Diagram
States:
- **S0**: Initial state
- **S1**: Detected `1`
- **S2**: Detected `10`
- **S3**: Detected `100`
- **S4**: Detected `1001` → Output = 1

Transitions based on `X` and `Z` with **1-bit overlap**.

---

## 📊 Example

| Input Stream (`X`) | Output (`Z`) |
|--------------------|--------------|
| 1                  | 0            |
| 0                  | 0            |
| 0                  | 0            |
| 1                  | 1 ✅         |
| 1                  | 0            |
| 1                  | 0            |
| 1                  | 0            |

> Sequence `"1001"` detected **twice** with **1-bit overlap**.

![1001 Mealy Machine Waveform](1001%20Sequence%20Detector%20%28Mealy%20Machine%29%20Waveform.png)

---

> 💡 This project demonstrates how sequential logic and state machines can be implemented using JK flip-flops — a foundational concept in digital design and VLSI FSM modeling.