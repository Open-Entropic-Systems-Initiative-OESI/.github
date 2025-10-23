<div align="center">

# ⚙️ **Adaptive Entropic System (AES)**  
### _A framework for energy–information balance in learning_  
#### Part of the [🌌 Open Entropic Systems Initiative (OESI)](https://github.com/<your-username>/Open-Entropic-Systems-Initiative)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)
[![Content License: CC BY-SA 4.0](https://img.shields.io/badge/Docs-CC%20BY--SA%204.0-brightgreen.svg)](./LICENSE-CONTENT)
[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/<your-username>/Adaptive-Entropic-System)
[![Charter](https://img.shields.io/badge/OESI-Scientific%20Charter-8A2BE2.svg)](./CHARTER.md)
[![Paper](https://img.shields.io/badge/Preprint-AES%20Paper-red.svg)](./paper/AES_Paper.pdf)

</div>

---

## 🔭 Overview
The **Adaptive Entropic System (AES)** is an open research framework implementing *entropic descent* — a thermodynamically grounded optimization process that couples **information compression** and **energetic efficiency**.  
AES demonstrates how learning systems can regulate themselves by minimizing excess energy while maximizing predictive coherence.

> “Persistence requires informational compression under energetic constraint.”

AES is developed as part of the [**Open Entropic Systems Initiative (OESI)**](https://github.com/<your-username>/Open-Entropic-Systems-Initiative),  
a broader effort to explore the physics of persistence, cognition, and emergence.

---


# Adaptive Entropic System (AES) — Colab Bundle

This bundle contains a Colab‑friendly implementation of the **Adaptive Entropic System (AES)**:
- self‑contained Python package `aes/`
- examples for MNIST, CIFAR‑10, and a 2D emergent simulation
- minimal tests and configs

## Quickstart (Colab)
1. Upload this zip to Colab and run:
```python
!unzip -o AES_Colab_Bundle.zip -d /content
%cd /content/AES_Colab_Bundle
!pip -q install -r requirements.txt
```
2. Run MNIST AES:
```python
!python examples/mnist_aes.py --epochs 3 --batch-size 256
```
3. Run the 2D emergent sim with live display:
```python
!python examples/sim2d_aes.py --steps 300 --show --save-gif sim.gif
```

## Notes
- GPU is auto‑detected; scripts fall back to CPU if needed.
- CIFAR loader uses `reshape()` not `view()` to avoid stride issues.
- You can change licenses later; defaults here are CC BY‑SA 4.0 (paper) and MIT (code).
