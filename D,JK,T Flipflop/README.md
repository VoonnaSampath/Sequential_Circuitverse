# D, T, JK Flip-Flops – CircuitVerse

## 🧠 Project Overview
This repository contains digital circuit designs of the **D**, **T**, and **JK Flip-Flops**, simulated on [CircuitVerse](https://circuitverse.org). These sequential logic circuits are essential in building registers, counters, and memory elements in digital systems.

## ✅ Key Features
- **D Flip-Flop**: Transfers the D input to Q on the rising edge of the clock.
- **T Flip-Flop**: Toggles the output Q on each clock pulse when T = 1.
- **JK Flip-Flop**: Combines the features of SR and T flip-flops; avoids invalid states.

### Inputs and Outputs

| Flip-Flop | Inputs       | Outputs      | Controlled by  |
|-----------|--------------|--------------|----------------|
| D         | D, Clock     | Q, Q'        | Clock Edge     |
| T         | T, Clock     | Q, Q'        | Clock Edge     |
| JK        | J, K, Clock  | Q, Q'        | Clock Edge     |

---

## 📊 Truth Tables

### 🔷 D Flip-Flop

| Clock | D | Q(next) |
|-------|---|---------|
| ↑     | 0 | 0       |
| ↑     | 1 | 1       |

> Q follows D at every rising edge of the clock.

---

### 🔷 T Flip-Flop

| Clock | T | Q(next) |
|-------|---|---------|
| ↑     | 0 | Q       |
| ↑     | 1 | Q̅       |

> Toggles output when T = 1 on the rising clock edge.

---

### 🔷 JK Flip-Flop

| Clock | J | K | Q(next) |
|-------|---|---|---------|
| ↑     | 0 | 0 | Q       |
| ↑     | 0 | 1 | 0       |
| ↑     | 1 | 0 | 1       |
| ↑     | 1 | 1 | Q̅       |

> When both J and K are high, the flip-flop toggles its state.

---

## 📂 Files Included

- `d_flipflop.cv` – CircuitVerse file for D Flip-Flop  
- `t_flipflop.cv` – CircuitVerse file for T Flip-Flop  
- `jk_flipflop.cv` – CircuitVerse file for JK Flip-Flop  
- `d_flipflop.png` – Schematic for D Flip-Flop  
- `t_flipflop.png` – Schematic for T Flip-Flop  
- `jk_flipflop.png` – Schematic for JK Flip-Flop  
- `README.md` – Project documentation

---

## 🔗 Live Simulations

- [D Flip-Flop](https://circuitverse.org/simulator/edit/d-flipflop-d4bb2b1c-c716-465a-b604-52f80ae38415)  
- [T Flip-Flop](https://circuitverse.org/simulator/edit/t-flipflop-807fbb7a-f5e0-414a-9f0d-a108834db7c4)  
- [JK Flip-Flop](https://circuitverse.org/simulator/edit/jk-flipflop-7defb4a7-8445-4adf-a537-f85b8041963e)

---

## 🛠 Tools Used
- [CircuitVerse](https://circuitverse.org) – Open-source digital logic design simulator