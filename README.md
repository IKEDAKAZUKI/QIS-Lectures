<div align="center">

# QIS Lectures

### Executable lecture notebooks for quantum information science and quantum programming

[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)
[![Qiskit](https://img.shields.io/badge/Qiskit-Quantum%20SDK-6929C4)](https://www.ibm.com/quantum/qiskit)
[![NumPy](https://img.shields.io/badge/NumPy-Linear%20Algebra-013243)](https://numpy.org/)
[![SciPy](https://img.shields.io/badge/SciPy-Scientific%20Computing-8CAAE6)](https://scipy.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

<br>

**Linear algebra · Qubits · Quantum gates · Measurements · Tensor products · CNOT · Bell states · Qiskit simulation**

</div>

---

## Overview

This repository contains introductory Jupyter notebooks for **quantum information science** and **quantum programming**.

The notebooks are designed as executable lecture material: students can read the explanations, run the code, modify examples, and directly observe the mathematical structures behind quantum computation.

The material begins with the linear-algebra foundations required for quantum information, then moves to gate-based quantum circuits using Qiskit.

This repository supplements lecture material at UMass Boston.

---

## Contents

| Topic | Notebook | Open in Colab |
|---|---|---|
| Linear algebra for quantum information | [`Linear Algebra.ipynb`](Linear%20Algebra.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IKEDAKAZUKI/QIS-Lectures/blob/main/Linear%20Algebra.ipynb) |
| Quantum circuits and gate operations | [`Gate operations.ipynb`](Gate%20operations.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IKEDAKAZUKI/QIS-Lectures/blob/main/Gate%20operations.ipynb) |

---

## Learning path

### 1. Linear Algebra

Start with:

```text
Linear Algebra.ipynb
```

This notebook introduces the basic mathematical language of quantum information using Python.

Topics include:

- complex numbers,
- complex vectors,
- vector addition,
- complex conjugation,
- inner products,
- norms,
- Pauli operators,
- sparse matrix representation,
- matrix addition and multiplication,
- Hermitian conjugation,
- unitary matrices,
- eigenvalues and eigenvectors.

This notebook is recommended before studying quantum circuits.

---

### 2. Gate Operations

Continue with:

```text
Gate operations.ipynb
```

This notebook introduces quantum programming with Qiskit.

Topics include:

- installing and importing Qiskit,
- creating quantum registers and classical registers,
- implementing a single qubit,
- measuring quantum states,
- applying one-qubit gates,
- visualizing circuits and results,
- rotating a qubit,
- computing tensor products,
- constructing two-qubit circuits,
- implementing CNOT gates,
- preparing Bell states,
- running circuits on a simulator.

The notebook also includes exercises on measurement, one-qubit rotations, tensor products, and two-qubit operations.

---

## Quick start

Clone the repository:

```bash
git clone https://github.com/IKEDAKAZUKI/QIS-Lectures.git
cd QIS-Lectures
```

Create a Python virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install --upgrade pip
```

For Windows PowerShell:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
```

Install the recommended packages:

```bash
python3 -m pip install qiskit qiskit-aer numpy scipy matplotlib pylatexenc jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Then open one of the notebooks:

```text
Linear Algebra.ipynb
Gate operations.ipynb
```

---

## Google Colab

The notebooks can also be opened directly in Google Colab using the badges above.

When running in Colab, execute the package-installation cells at the beginning of the notebook before running the remaining cells.

---

## Prerequisites

This repository is designed for students beginning quantum information science.

Recommended background:

- basic Python,
- elementary linear algebra,
- complex numbers,
- basic probability,
- interest in quantum mechanics or quantum computation.

No IBM Quantum account is required for the default simulator-based examples.

---

## What you will learn

After working through the notebooks, you should be comfortable with:

| Skill | Description |
|---|---|
| Linear-algebra computation | Use Python, NumPy, and SciPy to manipulate vectors, matrices, operators, eigenvalues, and eigenvectors |
| Quantum-state notation | Translate between Dirac notation, vectors, and computational-basis states |
| Pauli operators | Construct and manipulate the fundamental operators used in quantum information |
| Quantum circuits | Create quantum registers, classical registers, and Qiskit circuits |
| Measurement | Simulate quantum measurement and interpret shot-based outcomes |
| One-qubit gates | Apply basic gates and rotations to single-qubit states |
| Tensor products | Build multi-qubit Hilbert spaces from single-qubit systems |
| Two-qubit operations | Implement CNOT gates and create entangled Bell states |

---

## Local simulation

The quantum-circuit examples are simulator-based.

The main circuit notebook uses Qiskit and Qiskit Aer, so students can run the examples locally without access to real quantum hardware.

A typical simulator workflow is:

```python
from qiskit import QuantumCircuit, QuantumRegister, ClassicalRegister
from qiskit_aer import Aer

simulator = Aer.get_backend("qasm_simulator")
```

This makes the repository suitable for classroom use, self-study, and introductory demonstrations.

---

## Repository structure

```text
.
├── Gate operations.ipynb
├── Linear Algebra.ipynb
├── LICENSE
└── README.md
```

---

## Course context

This repository supplements lecture material for quantum information science and quantum programming at UMass Boston.

Related course page:

```text
https://courses.umb.edu/course_catalog/course_info/ugrd_PHYSIC_all_247
```

---

## Citation

If you use these notebooks for teaching, self-study material, or derivative lecture notes, please cite the repository:

```bibtex
@misc{IkedaQISLectures,
  author       = {Ikeda, Kazuki},
  title        = {QIS Lectures: Executable Lecture Notebooks for Quantum Information Science},
  year         = {2024},
  howpublished = {\url{https://github.com/IKEDAKAZUKI/QIS-Lectures}},
  note         = {Jupyter notebooks for quantum information science and quantum programming}
}
```

---

## License

This repository is released under the [MIT License](LICENSE).

Copyright (c) 2024 Kazuki Ikeda.

---

<div align="center">

**Quantum Information Science · Qiskit · Lecture Notebooks · Python**

</div>
