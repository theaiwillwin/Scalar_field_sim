# Scalar_field_sim

# Scalar Field Simulations

A multi-method simulation suite for modeling scalar field evolution in 2D domains. This toolkit supports experimental and comparative studies across finite-difference, spectral, and finite-element methods, including a framework for COMSOL automation.

---

## Features

- **Finite-Difference (SciPy + FFT)**
  - Explicit time-stepping with optional fractional Laplacian dynamics.
  - Incorporates mass term and external source capabilities.

- **Spectral Method (NumPy FFT)**
  - Implements fractional Laplacian on periodic domains via Fourier analysis.
  - Suitable for high-precision scalar diffusion or dispersion simulations.

- **Finite-Element Method (FEniCSx)**
  - Solves static scalar PDEs using the Helmholtz equation form.
  - Allows fine-grained mesh control and CG1 basis support.

- **COMSOL Automation (mph pseudo-script)**
  - Intended for use with the `mph` Python API for COMSOL Multiphysics.
  - Outlines scalar field setup for interactive or batch simulations.

---

## Requirements

- Python 3.10+
- [NumPy](https://numpy.org)
- [SciPy](https://scipy.org)
- [Matplotlib](https://matplotlib.org)
- [FEniCSx](https://fenicsproject.org)
- [mpi4py](https://mpi4py.readthedocs.io)
- Optional: COMSOL Multiphysics + `mph` Python package

Install all dependencies with:

```bash
pip install -r requirements.txt
