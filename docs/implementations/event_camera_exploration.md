# Event Camera Data Exploration

**Date:** April 2026
**Notebook:** `Day1_EventCameras.ipynb`
**Dataset:** N-MNIST (neuromorphic MNIST via `tonic` library)

---

## What I built

Loaded and visualised real event camera data for the first time. N-MNIST is the standard MNIST digit dataset captured by moving a DVS camera in front of static handwritten digits, producing a stream of events rather than frames.

---

## Key things I learned

**The event format.** Each event is `(x, y, t, p)` — pixel position, microsecond timestamp, and polarity (ON/OFF). The data is a structured numpy array, not an image tensor.

**Sparsity.** On average only ~[fill in %] of pixels are active at any time bin. This is the core efficiency property — most of the sensor is silent most of the time.

**Event frames.** Converting raw events to a `[T, 2, H, W]` tensor using `tonic.transforms.ToFrame(n_time_bins=10)` gives you the format an SNN can process. T time steps map directly to T forward passes through the network.

---

## Visualisations produced

- Scatter plot of all events coloured by timestamp — the digit shape is visible in the spatial distribution
- ON vs OFF polarity separated — shows the edges of the digit moving
- Event density heatmap — accumulation over all time steps
- 10-bin event frame sequence — the digit revealed over time

---

## What surprised me

*[Fill in after completing the notebook]*

---

## Connection to the project

This is the input format for Task 1. Every SNN I build will consume tensors in the `[T, 2, H, W]` format produced here. Understanding the sparsity structure is also directly relevant to why the hardware (RTD NanoLEDs) is a good match — both the data and the hardware are spike-based and sparse.

---

## What I'd do differently

*[Fill in after completing the notebook]*
