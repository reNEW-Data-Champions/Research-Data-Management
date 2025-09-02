---
layout:
  width: wide
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# 🟠 DAN HPC Hub

## DAN HPC System Overview

The **DAN System** is a High-Performance Computing (HPC) environment owned by **reNEW** (The Novo Nordisk Foundation Center for Stem Cell Medicine, SUND, University of Copenhagen) and designed to support computational experts who require access to large-scale datasets stored on **KU-IT storage** for advanced processing.

The platform is optimized for **genomics** and **image data analysis** workflows, enabling researchers to leverage powerful CPU and GPU resources for intensive computational tasks.

The system includes:

* **1 GPU computing node** for image data analysis
* **2 high-capacity CPU computing nodes** for genomics data analysis
* Resources contributed by reNEW collaborators:
  * **CGEN** – Center for Gene Expression
  * **CPR** – Novo Nordisk Foundation Center for Protein Research
* Integration with KU-IT storage for direct access to large datasets
* Managed using **SLURM Workload Manager** for efficient job scheduling
* Co-administered with KU to ensure optimal uptime and performance

This shared HPC infrastructure enhances computational capacity across the **Faculty of Health and Medical Sciences (SUND)**, accelerating research requiring large-scale data processing.

***

## DAN HPC System Specifications

<table><thead><tr><th width="228">Node Name</th><th width="396">CPU Configuration</th><th>GPU Configuration</th><th width="85">RAM</th><th width="305">Operating System</th><th>Role</th></tr></thead><tbody><tr><td><strong>Head Node</strong><code>danhead01fl</code></td><td>6 virtual CPUs</td><td>—</td><td>12 GB</td><td>Red Hat Enterprise Linux 8 + SLURM</td><td>Login/control node</td></tr><tr><td><strong>GPU Node</strong><code>dangpu01fl</code></td><td>4 × Intel Xeon Platinum 8280 @ 2.70 GHz224 cores/threads (Hyper-threading)</td><td>4 × NVIDIA Quadro RTX 8000</td><td>4 TB</td><td>Red Hat Enterprise Linux 8 + SLURM</td><td>Compute node, Jupyter/RStudio server</td></tr><tr><td><strong>CPU Node 01</strong><code>dancmpn01fl</code></td><td>2 × AMD EPYC 7763 @ 2.45 GHz256 cores/threads (Hyper-threading)</td><td>—</td><td>4 TB</td><td>Red Hat Enterprise Linux 8 + SLURM</td><td>Compute node</td></tr><tr><td><strong>CPU Node 02</strong><code>dancmpn02fl</code></td><td>2 × AMD EPYC 9454 @ 2.75 GHz192 cores/threads (Hyper-threading)</td><td>—</td><td>768 GB</td><td>Red Hat Enterprise Linux 8 + SLURM</td><td>Compute node</td></tr></tbody></table>

***

**For more information:** Contact **Sen Li** or visit the [DanGPU website](https://sgn102.pages.ku.dk/a-not-long-tour-of-dangpu/).

