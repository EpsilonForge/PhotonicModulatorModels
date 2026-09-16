---
title: Photonic Modulator Models
description: A collection of notes and analytic models to demostrate different principles of photonic modulation technology.
---

# Photonic Modulator Models

Executable notes on silicon photonic modulators, published as a [MyST](https://mystmd.org) website on GitHub Pages.

The full study lives in [the semiconductor notebook](./semiconductor.ipynb).

## Contents

- **General concepts** — bands, effective mass, Drude picture
- **Equilibrium concentrations** — intrinsic/extrinsic carriers, Poisson–Boltzmann solution, Sze depletion approximation
- **Biased junction** — Poisson + drift-diffusion + SRH recombination, steady-state IV, charge, dynamic conductance/capacitance
- **Optical properties** — Sellmeier index, Franta data, Drude free-carrier $\Delta n$ / $k$ at 1550 nm

## Run locally

```bash
pip install -r requirements.txt
npm install -g mystmd   # or: pip install mystmd
myst start              # preview with stored outputs
myst start --execute    # re-execute the notebook
myst build --html       # static build in _build/html
myst build --execute --html  # re-execute, then build
```

Python dependencies are listed in `requirements.txt` (`numpy`, `scipy`, `matplotlib` plus `jupyter-server`/`ipykernel` for `--execute`).

## Deploy

Pushes to `main` trigger `.github/workflows/deploy.yml`, which builds with `myst build --execute --html` and deploys `_build/html` to GitHub Pages.
Enable it once under **Settings → Pages → Source: GitHub Actions**.
The site is served at `https://<org>.github.io/PhotonicModulatorModels/`.
