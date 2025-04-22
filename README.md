# Quantum Teleportation – Qiskit Project  
**University Quantum Computing Project**  
*Topic: Introduction to Near-Term Quantum Computing*  
**Date:** April 2025  

---

## 📚 Table of Contents
- [Project Overview](#project-overview)
- [Setup & Requirements](#setup--requirements)
- [Section Highlights](#section-highlights)
  - [1. Single-Qubit Quantum Gates](#1-single-qubit-quantum-gates)
  - [Exercise 1 – Build Quantum Circuits](#exercise-1--build-quantum-circuits)
  - [2. Multi-Qubit Quantum Gates](#2-multi-qubit-quantum-gates)
  - [3. Run on a Real Quantum Device](#3-run-on-a-real-quantum-device)
  - [4. Quantum State Tomography](#4-quantum-state-tomography)
  - [Exercise 2 – Estimate Bloch Sphere Coordinates](#exercise-2--estimate-bloch-sphere-coordinates)
  - [5. Quantum Teleportation](#5-quantum-teleportation)
  - [Exercise 3 – Build a Teleportation Circuit](#exercise-3--build-a-teleportation-circuit)

---

## 📖 Project Overview
This project explores the principles of quantum computation with a focus on **Quantum Teleportation**, using IBM's Qiskit framework. The implementation includes simulations, visualizations, and real-device execution. The exercises aim to build intuition around quantum gates, entanglement, and the behavior of quantum states.

---

## 🛠 Setup & Requirements

### Required Packages
Run the following if you're using Google Colab:
```python
# %pip install qiskit[visualization]
# %pip install qiskit-aer
# %pip install qiskit-ibm-runtime
```

### Version Check
```python
import qiskit
qiskit.__version__
```

---

## 🔍 Section Highlights

### 1. Single-Qubit Quantum Gates
- Basic gates: `X`, `H`, `Z`
- Use of `StatevectorSimulator` and `plot_bloch_multivector`
- Constructing and visualizing states like `|0⟩`, `|1⟩`, `|+⟩`, and `|−⟩`

---

### 🧪 Exercise 1 – Build Quantum Circuits
- Apply quantum gates to explore state transformations
- Examples: `XX|0⟩`, `HH|0⟩`, `HZH|0⟩`
- Bloch sphere visualization for each case

---

### 2. Multi-Qubit Quantum Gates
- Two-qubit circuits and tensor products
- Equal superposition using `H` gates
- Understanding bit order in Qiskit (Little Endian)

---

### 3. Run on a Real Quantum Device
- Follow the **Qiskit Patterns**:
  1. Map the problem to a quantum-native format
  2. Optimize circuit for hardware
  3. Execute the circuit
  4. Postprocess results
- Creation and measurement of Bell states

---

### 4. Quantum State Tomography
- Estimating qubit states using measurement statistics
- Calculation of `(r_x, r_y, r_z)` coordinates
- Visualization with Bloch vectors

---

### 🧪 Exercise 2 – Estimate Bloch Sphere Coordinates
- Build circuits to estimate `r_z`, `r_x`, `r_y`
- Use transformations (e.g., `H`, `S†`) before measurement
- Compare estimated values with original random state

---

### 5. Quantum Teleportation
- Implementation of a full teleportation protocol
- Use of entanglement, mid-circuit measurement, and conditional gates
- Final state verification using `u-gate` inverse
- Execution on both simulator and real backend

---

### 🧪 Exercise 3 – Build a Teleportation Circuit
- Construct a 3-qubit teleportation circuit from scratch
- Follow full Qiskit Patterns lifecycle
- Post-process real device results and extract target qubit state

---

## 🧠 Notes
- Qiskit uses **Little Endian** (qubit 0 = rightmost bit)
- Measurement noise and decoherence affect real hardware
- Use `plot_histogram()` and `plot_bloch_multivector()` for validation

---

## 📎 Resources
- [Qiskit Docs](https://qiskit.org/documentation/)
- [IBM Quantum Platform](https://quantum.ibm.com/)
- [Qiskit Circuit API](https://docs.quantum.ibm.com/api/qiskit/qiskit.circuit.QuantumCircuit)

---

> This project was created as part of a university-level exploration in quantum computing using IBM's Qiskit SDK.
