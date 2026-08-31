# Neutron Star EOS Density Solver

Numerically solves the TOV equations for neutron stars, computing radial density profiles across different equations of state.

## Overview

Inside a neutron star, gravity pulls matter inward while pressure from dense nuclear matter pushes back outward. Because conditions are extreme enough for general relativity to matter, this balance is described by the Tolman-Oppenheimer-Volkoff (TOV) equations rather than the simpler Newtonian version.

This project integrates the TOV equations outward from the center of the star (given a central density and an equation of state) until the pressure drops to zero — marking the star's surface. This gives the density profile, along with the resulting mass and radius.

## Results

- **Density profile** — how density falls off from the center to the surface
- **Parameter dependence** — how the profile and mass-radius relation change across different values of the equation-of-state parameter `a`


<img width="580" height="437" alt="image" src="https://github.com/user-attachments/assets/5c9c4620-28d4-4018-86a2-d4d10cfacab0" />

<img width="589" height="437" alt="image" src="https://github.com/user-attachments/assets/b4f81019-07f8-4db9-8ac3-971c5f44678f" />


## Usage

```bash
pip install numpy scipy matplotlib
jupyter notebook neutron_star.ipynb
```

Adjust the central density or equation-of-state parameters in the notebook to try different configurations.

## Dependencies

- numpy
- scipy
- matplotlib

## References

- Tolman (1939), *Static Solutions of Einstein's Field Equations for Spheres of Fluid*
- Oppenheimer & Volkoff (1939), *On Massive Neutron Cores*
