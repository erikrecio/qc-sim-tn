# qc-sim-tn  
Code accompanying the thesis **“Simulating Quantum Computers with Tensor Networks”** (Erik Recio, 2022)

This repository contains Julia code, raw outputs, and plots used to study tensor-network simulation of variational quantum circuits for state **decoding/disentangling** (reverse-VQE style), with focus on observables such as **magnetization** and **entanglement entropy**.

## Related work

- **Master Thesis:** *Simulating Quantum Computers with Tensor Networks* (University of Barcelona / ICFO, Sept 2022)

## Repository layout (tailored to current `main`)

```text
qc-sim-tn/
├── Old/                               # Older experiments / archived code
├── Plots/                             # Figure outputs
├── Results/                           # Experiment results
├── .gitignore
├── Code TFM.jl                        # Main thesis code (Julia)
├── README.md                          # This readme
└── plots.py                           # Script to create the plots of the thesis
```

## Setup

This project is Julia-based.

```bash
julia --version
```

Install typical packages from Julia REPL:

```julia
using Pkg
Pkg.add(["LinearAlgebra", "Statistics", "DelimitedFiles", "Plots"])
```

## Usage

Run the main thesis script:

```bash
julia "Code TFM.jl"
```

Outputs are typically written to `Results/` and figures to `Plots/`.

## Scientific scope

The codebase is aligned with the thesis pipeline:

- tensor-network representation (MPS perspective),
- reverse-variational decoding of Ising ground states,
- analysis of performance against circuit depth / system size,
- evaluation via magnetization and von Neumann entropy.

## Citation

If you use this repository, cite the thesis:

```text
Erik Recio, Simulating Quantum Computers with Tensor Networks,
Institute of Photonic Sciences (ICFO), September 2022.
```

and link this repository in your methods/code availability section.
