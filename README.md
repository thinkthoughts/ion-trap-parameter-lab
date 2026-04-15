# Ion Trap Parameter Lab

Numerical tools for modeling and optimizing surface-electrode ion traps.

## Overview

This project develops lightweight, reproducible workflows for ion trap design, focusing on:

- Electrostatic potential and field calculations (Laplace / Poisson)
- RF pseudopotential analysis
- Multi-parameter sweeps (geometry, voltages)
- Stability and confinement region identification
- Basic optimization of trap configurations

The goal is to connect physical modeling with practical design intuition for trapped-ion quantum systems.

## Quick Start

### Option 1: Run in Colab
Click the button below to open the first notebook:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](REPLACE_WITH_NOTEBOOK_LINK)

### Option 2: Local setup

```bash
git clone https://github.com/thinkthoughts/ion-trap-parameter-lab.git
cd ion-trap-parameter-lab

# using pip
pip install -r requirements.txt

# OR using conda
conda env create -f environment.yml
conda activate ion-trap-parameter-lab

jupyter lab
```

## Framework

This project is guided by a general constraint-based workflow:

- Define a parameter domain  
- Apply finite physical and design constraints  
- Identify regions that remain stable and bounded under numerical verification  

This approach is informed by: https://sdg5.app/main.pdf

In that work, bounded structure emerges from finite constraints rather than unbounded filtering.  
Here, the same idea is applied to ion-trap parameter spaces to identify stable confinement regions.

## Structure (initial)

- `notebooks/` — simulation and visualization workflows  
- `src/` — reusable numerical components (solvers, utilities)  
- `figures/` — generated plots and diagrams  

## Status

Early-stage. Initial notebooks will implement electrostatic solvers and simple trap geometries.

## Related Work

- Rydberg simulations → https://github.com/thinkthoughts/rydberg-parameter-lab  
- Ion benchmarking → https://github.com/thinkthoughts/ion-benchmark-lab  
