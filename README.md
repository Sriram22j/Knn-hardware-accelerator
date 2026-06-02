# KNN Hardware Accelerator

## Overview

This project implements a **K-Nearest Neighbors (KNN) Hardware Accelerator** using **Verilog HDL** for FPGA-based machine learning acceleration.

The accelerator is designed using a modular RTL architecture and performs KNN classification through hardware-accelerated distance computation, Top-K neighbor selection, and majority voting. The design is optimized for parallel processing and low-latency inference.

### Key Highlights

* Designed and implemented a pipelined KNN accelerator using synthesizable Verilog RTL.
* Implemented a distance computation engine, Top-K selector, and majority voting modules.
* Integrated instruction-driven control architecture with decoder and program counter.
* Verified functionality using **ModelSim simulations**.
* FPGA-compatible modular hardware design.

---

## Features

* Hardware implementation of the KNN algorithm
* Parallel distance computation
* Top-K nearest neighbor selection
* Majority-voting based classification
* Modular RTL architecture
* FPGA deployment support
* Performance monitoring using latency counter

---

## Architecture

The accelerator consists of the following modules:

### Distance Engine

Computes the distance between the query sample and all training samples.

### Top-K Selector

Selects the K nearest neighbors based on computed distances.

### Voting Logic

Determines the final classification result using majority voting.

### Instruction Memory

Stores instructions controlling accelerator operation.

### Program Counter (PC)

Controls instruction sequencing.

### Decoder

Decodes instructions and generates control signals.

### Latency Counter

Measures execution cycles and accelerator performance.

---

## Project Structure

```text
knn-hardware-accelerator
├── src
│   ├── knn_processor_top.v
│   ├── knn_system_l.v
│   ├── pc.v
│   ├── decoder.v
│   ├── distance_engine.v
│   ├── top_k_selector.v
│   ├── voting_logic.v
│   └── latency_counter.v
│
├── testbench
│   └── tb_knn_system.v
│
├── memory
│   ├── query.mem
│   ├── instruction_memory.v
│   └── training_data.v
│
└── README.md
```

---

## Tools Used

* Verilog HDL
* ModelSim
* Intel Quartus Prime

---

## Simulation Flow

1. Compile all RTL modules.
2. Compile the testbench (`tb_knn_system.v`).
3. Load memory initialization files.
4. Run simulation in ModelSim.
5. Observe classification results and latency measurements.

---

## Applications

* Machine Learning Acceleration
* Edge AI Systems
* FPGA-Based AI Inference
* Real-Time Classification Systems
* Embedded AI Applications

---



## Author

**Sriram J**


