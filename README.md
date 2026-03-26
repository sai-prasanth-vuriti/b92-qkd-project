# B92 Quantum Key Distribution (QKD) Simulator

## Overview

This project simulates the B92 Quantum Key Distribution protocol to demonstrate secure key exchange using principles of quantum mechanics.
It includes eavesdropping detection, performance analysis, and secure key generation.
---
## Features

B92 QKD Protocol Simulation
Intercept-Resend Attack (Eavesdropping)
Quantum Bit Error Rate (QBER) Calculation
Key Generation Efficiency Analysis
Privacy Amplification using SHA-256
User Mode and Analysis Mode

---
## Working Principle

Bit 0 is encoded as |+⟩ (X-basis)
Bit 1 is encoded as |1⟩ (Z-basis)
Bob measures using randomly chosen Z or X basis
Only conclusive results (about 25%) are retained
If QBER ≥ 11%, the channel is considered compromised
---
## How to Run

Install dependencies
pip install qiskit qiskit-aer matplotlib

Run the program
python b92.py

Select mode
1 → User Mode
2 → Analysis Mode
3 → Demo Mode (Attack vs No Attack)
---
## Output
Key length and efficiency
QBER values
Security status (Secure / Compromised)
Graphs for efficiency and QBER

## Expected Results
No attack: QBER close to 0, secure communication
With attack: QBER around 25%, communication aborted
---
## Security Insight

The protocol ensures security because any attempt to measure quantum states disturbs them, which increases QBER and reveals the presence of an eavesdropper.

Technologies Used
Python
Qiskit (conceptual simulation)
Matplotlib
