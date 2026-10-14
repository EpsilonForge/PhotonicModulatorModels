---
title: Photonic Modulator Models
description: A collection of notes and analytic models to demostrate different principles of photonic modulation technology.
---

# Photonic Modulator Models

Executable notes on silicon photonic modulators.

This collection of notebooks intends to serve as a textbook-style reference of simple analytic models that explain the fundamental physics of photonic modulators and related devices. The goal is to build intuition by deriving each result from first principles and then making it concrete with a small, self-contained Python implementation that the reader can run and modify.

The notes begin with a [biased p–n junction](./pn_junction.ipynb), covering the general properties of semiconductors, carrier statistics in intrinsic and extrinsic material, the equilibrium carrier concentrations, and the coupled Poisson, drift-diffusion and generation–recombination equations that describe the junction away from equilibrium. 

Then, we move to a [carrier-depletion p–n junction phase shifter](./pn_junction_phase_shifter.ipynb), where the abrupt-junction electrostatics and the depletion approximation are combined with the optical properties of doped silicon — including the free-carrier Drude contribution to the refractive index — and with the lateral modes of a ridge waveguide to obtain the phase shift produced by the depletion region.

Together the notebooks trace the path from basic semiconductor physics to the optical response of a silicon modulator. They are written to be read in order, while each remains self-contained and can be run on its own.

