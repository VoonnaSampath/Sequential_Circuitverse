# "1001" Moore Sequence Detector with 1-bit Overlap – CircuitVerse

## 🧠 Project Overview
This project implements a **Moore-type finite state machine (FSM)** to detect the binary sequence **"1001"** in a serial input stream. The design uses **JK flip-flops** to hold the state and allows **1-bit overlapping**, enabling the FSM to detect sequences that share bits. Designed and simulated using [CircuitVerse](https://circuitverse.org), this system is ideal for real-time digital pattern recognition.

## ✅ Key Features
- **Functionality**: Detects the binary sequence `"1001"` using a Moore FSM model
- **Design Type**: Moore machine with 1-bit overlap
- **Flip-Flops Used**: JK Flip-Flops for state encoding
- **Inputs**:
  - `X` – Serial 1-bit input
  - `CLK` – Clock signal
- **Outputs**:
  - `Output` – Output goes HIGH (1) when the full sequence is detected (associated with a state)

## 📂 Files Included
- `1001 Moore Sequence Detector with 1 Bit Overlapping.cv` – Raw exported CircuitVerse file
- `1001 Moore Sequence Detector with 1 Bit Overlapping.png` – Schematic diagram of the detector circuit
- `README.md` – Markdown documentation for the project

## 🔗 Live Simulation
[Click here to view the project on CircuitVerse](https://circuitverse.org/simulator/edit/1001-moore-sequence-detector-with-1-bit-overlapping)

## 🛠 Tools Used
- [CircuitVerse](https://circuitverse.org) – Online digital circuit simulator

---

## 🧩 How the Moore Sequence Detector Works

In a Moore machine, the output depends **only on the current state**. For the "1001" sequence detector:

### 📐 FSM States:
- **S0**: Start state
- **S1**: Received `1`
- **S2**: Received `10`
- **S3**: Received `100`
- **S4**: Received full `1001` → `Z = 1` (output associated with this state)

### 🔁 Transitions:
- On each clock pulse, the FSM transitions based on input `X`
- When state `S4` is reached, `Z = 1`
- On overlap, it reuses the final `1` to re-enter S1

---

## 📊 Example

| Clock Cycle | Input (X) | State | Output (Z) |
|-------------|-----------|--------|-------------|
| 1           | 1         | S1     | 0           |
| 2           | 0         | S2     | 0           |
| 3           | 0         | S3     | 0           |
| 4           | 1         | S4     | 1 ✅        |
| 5           | 0         | S2     | 0           |
| 6           | 0         | S3     | 0           |
| 7           | 1         | S4     | 1 ✅        |

> The Moore machine sets the output **after** reaching the final state, thus a 1-cycle delay compared to Mealy model.

---

## 🖼 Waveform or Simulation Screenshot

```markdown
![1001 Moore Sequence Detector Waveform](1001%20Moore%20Sequence%20Detector%20with%201%20Bit%20Overlapping%20Waveform.png)