# Implementations

Every piece of code I've built, with context, results, and honest notes on what went wrong.

---

## Event-Based Vision

| Implementation | Dataset | Key Result | Notebook | Status |
|----------------|---------|------------|----------|--------|
| [Event Camera Data Exploration](event_camera_exploration.md) | N-MNIST | Visualised raw events, event frames, sparsity | Day1_EventCameras.ipynb | ✅ Done |

---

## Spiking Neural Networks

| Implementation | Dataset | Key Result | Notebook | Status |
|----------------|---------|------------|----------|--------|
| [First SNN Classifier](snn_nmnist.md) | N-MNIST | — | — | ⏳ Pending |
| [SNN on DVS Gesture](snn_dvs_gesture.md) | DVS128 Gesture | — | — | ⏳ Pending |
| [Edge Detection — Hejda et al. 2022](edge_detection_rtd.md) | — | — | — | ⏳ Pending |

---

## Hardware Models

| Implementation | Based On | Description | Status |
|----------------|----------|-------------|--------|
| [RTD Neuron ODE Simulation](rtd_ode_model.md) | Ortega-Piwonka et al. 2021 | Simulate RTD spiking dynamics in Python | ⏳ Pending |
| [Custom RTD Neuron in snnTorch](rtd_snntorch_layer.md) | Romeira 2023 + RTD papers | Replace LIF with RTD dynamics | ⏳ Pending |
