# D²-UC: A Distributed–Distributed Quantum–Classical Framework for Unit Commitment

![License](https://img.shields.io/badge/license-Academic-blue)
![Python](https://img.shields.io/badge/python-3.10%2B-blue)
![Qiskit](https://img.shields.io/badge/Qiskit-0.39.0-purple)

> Official code, data, and results accompanying the paper:  
> *"D²-UC: A Distributed–Distributed Quantum–Classical Framework for Unit Commitment"*   

---

## 🔬 Overview

This repository contains implementations, datasets, and results for our **quantum-ready Unit Commitment (UC) framework**.  
We reformulate deterministic and stochastic UC into a **three-block ADMM** with Block 2 cast as a **QUBO** problem.  
These QUBOs are then solved using both brute force and the **Distributed Variational Quantum Eigensolver (DVQE)**.

Our framework supports:
- Three decomposition modes: three-QUBO, micro-QUBO, and batched-QUBO
- Hybrid quantum–classical execution of UC subproblems
- Validation across **small (3 units)**, **medium (20 units)**, and **large (50 units)** UC systems

All numerical experiments, figures, and dispatch tables in the paper can be reproduced here.

---

## 🌟 Features

- **Three-Block ADMM** decomposition for UC (dispatch, binary QUBO, consensus)  
- **QUBO Decomposition Strategies**: three-QUBO, micro-QUBO, and batched-QUBO  
- **DVQE Solver Integration** with accept-if-better safeguard  
- **Benchmarking** against brute force oracle solutions  
- **Scalable Validation** on deterministic and stochastic UC problems  

---

## 📚 Citation

If you use the content of this project in your research, please cite:

> M. Hasanzadeh and A. Kargarian, "D²-UC: A Distributed–Distributed Quantum–Classical Framework for Unit Commitment," [https://arxiv.org/abs/2508.17471](https://arxiv.org/abs/2511.03104)


---

## 👤 Author

**Milad Hasanzadeh**  
Department of Electrical and Computer Engineering  
Louisiana State University  
📧 e.mhasanzadeh1377@yahoo.com  

📅 **Release Date:** Nov 2025  
📄 **License:** Academic and Research Use Only  

---

## 📦 Installation

Clone this repo and install dependencies.  
DVQE must be installed from our official repository:

```bash
# Install DVQE
pip install git+https://github.com/LSU-RAISE-LAB/DVQE.git

# Clone this repo
git clone https://github.com/LSU-RAISE-LAB/3B-ADMM-UC-DVQE.git
cd 3B-ADMM-UC-DVQE

# Install required packages
pip install -r requirements.txt



