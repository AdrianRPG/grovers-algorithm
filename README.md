# 🔍 Grover’s Search Algorithm (Quantum Computing with Qiskit)

## 📌 Project Overview
This project implements **Grover’s Search Algorithm** using Qiskit to efficiently search for a target value within an unstructured dataset of 16 elements.

The algorithm demonstrates **quantum speedup**, reducing search complexity from classical **O(N)** to **O(√N)**.

---

## 🎯 Objective
- Simulate Grover’s Algorithm on a 4-qubit search space (16 elements)
- Compare classical vs quantum search performance
- Understand key quantum concepts such as:
  - Superposition
  - Phase kickback
  - Amplitude amplification

---

## ⚙️ Technologies & Tools
- Python
- Qiskit
- Qiskit Aer Simulator
- Jupyter Notebook
- NumPy
- Matplotlib

---

## 🧠 Key Concepts Implemented

### 1. Data Embedding
Classical data is encoded into quantum states using controlled operations.

### 2. Oracle (Phase Inversion)
Marks the correct solution by applying a phase flip using **phase kickback**.

### 3. Uncomputation
Reverses the data embedding to remove entanglement and isolate the marked state.

### 4. Diffuser (Amplitude Amplification)
Amplifies the probability of the correct solution using reflection about the mean.

### 5. Measurement
Extracts the most probable state (correct index) from the quantum system.

---

## 🔄 Algorithm Workflow

1. Initialize qubits in superposition  
2. Encode classical data into quantum states  
3. Apply oracle to mark the target value  
4. Uncompute to clean entanglement  
5. Apply diffuser to amplify the correct state  
6. Repeat steps 2–5 for optimal iterations  
7. Measure the address qubits  

---

## 📊 Results

- The algorithm successfully identifies the correct index with high probability
- Optimal number of iterations used: iterations = ((π / 4) * √(N / M))
- Measurement results show a dominant peak at the correct state

---

## 📈 Example Output
- Expected index: 1010
- Most probable result: 1010

Histogram visualization confirms the correct result with high probability.

---

## 🚀 Skills Demonstrated

- Quantum algorithm implementation
- Circuit design using Qiskit
- Reversible computation (uncomputation)
- Problem decomposition and algorithmic thinking
- Simulation and result validation

---

## 📁 Project Structure

---

## ▶️ How to Run

1. Install dependencies:
```bash
pip install qiskit matplotlib numpy
```
2. Open the notebook:
```bash
jupyter notebook Grover_Algorithm_Perez_Galindo_Adrian.ipynb
```
3. Run all cells
