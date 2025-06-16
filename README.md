# Verilog-ML Anomaly Detector 🧠🔧

This project explores how machine learning can accelerate functional verification in digital hardware design by **detecting anomalies** in Verilog simulation outputs. The goal is to build an intelligent tool that learns from correct simulation behavior and flags deviations in faulty or modified circuits.

> Think of it as an AI-powered junior verification engineer — observing patterns, learning signal behavior, and catching bugs.

---

## 🔍 Project Objective

To build a prototype tool that:
- Takes **Verilog simulation data** (e.g., counters, FSMs)
- Learns “correct” output waveforms via ML
- **Flags abnormal behavior** in faulty designs
- Scales across multiple modules (ALU, UART, etc.)
- Could one day plug into EDA toolchains

---

## 📁 Repo Structure

```bash
verilog-ml-anomaly-detector/
├── verilog_modules/        # All Verilog designs and testbenches
├── simulation_outputs/     # CSV waveform outputs (ModelSim, Icarus, etc.)
├── ml_model/               # ML code, notebooks, preprocessing
├── results/                # Model performance, prediction plots
├── docs/                   # Project timeline, references, paper summaries
└── README.md               # This file
