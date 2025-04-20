# Quantum Circuit Simulator with Graph Partitioning and Parallel Tensor Contraction

A distributed quantum circuit simulation framework that leverages **graph partitioning (METIS)**, **multi-node parallelism (MPI)**, and **intra-node acceleration (OpenCL/OpenMP)** to scale tensor network contractions for large quantum circuits.

---

## 🚀 Project Overview

This project simulates quantum circuits by modeling them as **tensor networks** and contracting them using parallel resources across multiple compute nodes.

- **Graph-based approach**: Exploits the graph structure of quantum circuits.
- **Distributed Execution**: Partitions the circuit into subgraphs across MPI ranks.
- **Accelerated Contraction**: Uses OpenCL or OpenMP for local tensor contraction steps.
- **Scalable & Modular**: Designed to run on lab clusters or cloud-based VM environments.

---

## 🧠 Core Strategy

| Layer              | Technology         | Purpose                                                                 |
|-------------------|--------------------|-------------------------------------------------------------------------|
| Circuit Frontend  | Julia (QXTools)    | Circuit definition and orchestration                                   |
| Partitioning       | METIS              | Graph partitioning and community detection                             |
| Inter-node Comm   | MPI                | Distributes subgraphs and synchronizes contraction stages              |
| Intra-node Compute| OpenCL / OpenMP    | Accelerated tensor contraction (OpenCL for GPUs, OpenMP for CPUs)      |

---
## [Link to Presentation](https://docs.google.com/presentation/d/15YkYsFm8WkFIVgqzzwpQaJmRpNWMUCb37mfhM6RkPaM/edit?usp=sharing)

