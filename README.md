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
## 📆 Project Timeline (July 28 – November 30, 2025)

### 🔹 Phase 1: Foundation (July 28 – August 15)
- [ ] Choose and simulate a basic Verilog module (e.g., 4-bit counter, FSM)
- [ ] Extract simulation data to CSV (using Icarus Verilog, ModelSim, etc.)
- [ ] Study waveform patterns and structure data for ML usage
- [ ] Label datasets as “normal” vs “bug-injected”

### 🔹 Phase 2: ML Integration (August 16 – September 10)
- [ ] Select appropriate ML algorithm (Logistic Regression, SVM, or RNN)
- [ ] Train and validate the model on waveform data
- [ ] Test model performance with functional bug-injected designs
- [ ] Evaluate metrics (Accuracy, Precision, Recall, F1 Score)

### 🔹 Phase 3: Multi-Module Generalization (September 11 – October 5)
- [ ] Extend project to more Verilog modules (ALU, UART, FIFO, etc.)
- [ ] Improve waveform pre-processing pipeline
- [ ] Build a reusable CSV-to-input-data pipeline for different modules
- [ ] Prepare scripts to automatically flag anomalous simulation runs

### 🔹 Phase 4: Tool Development & Documentation (October 6 – November 15)
- [ ] Build a CLI tool (or minimal GUI) to interact with the anomaly detector
- [ ] Add code comments, organize repo folders, write usage guides
- [ ] Draft a publishable EFY-style article documenting the project
- [ ] Record demo videos and screenshots for presentation

### 🔹 Phase 5: Final Polish & Publishing (November 16 – November 30)
- [ ] Final code cleanup, bug fixes, and refactoring
- [ ] Push final version to GitHub (make repo public)
- [ ] Add GitHub to resume + LinkedIn
- [ ] Optional: Submit article to EFY / write blog on Medium
## 📁 Repo Structure

```bash
verilog-ml-anomaly-detector/
├── verilog_modules/        # All Verilog designs and testbenches
├── simulation_outputs/     # CSV waveform outputs (ModelSim, Icarus, etc.)
├── ml_model/               # ML code, notebooks, preprocessing
├── results/                # Model performance, prediction plots
├── docs/                   # Project timeline, references, paper summaries
└── README.md               # This file
