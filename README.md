# Unsteady Vortex Lattice Method (UVLM) Analysis of Rotating Blades

## Overview
This project investigates unsteady aerodynamic behaviour using the Unsteady Vortex Lattice Method (UVLM), with application to moving lifting surfaces and rotating blades.

The work focuses on numerical simulation and validation of aerodynamic loads in time-dependent configurations, with particular attention to rotor aerodynamics.

Results are compared against published benchmark data to verify the reliability of the simulations.

---

## Benchmark Reference
Simulations were validated against the benchmark cases presented in:


**Verstraete et al., 2023** – "Code-to-Code Benchmark for Simulation Tools Based on the Unsteady Vortex-Lattice Method," 
*Journal of Aerospace Information Systems*, 20(11), 719–746.

This project reproduces and analyses benchmark configurations, with particular focus on **Case 4 (two-blade rotor)**.  
Additional benchmark cases (including static and prescribed-motion flat plates) were also simulated.

---

## Objectives
- Apply UVLM to unsteady aerodynamic configurations
- Simulate rotating lifting surfaces
- Compare numerical results with benchmark reference data
- Analyse the influence of the blade angle of attack and the vertical freestream velocity
- Adapt an existing UVLM implementation to handle rotating geometries

---

## Methodology

### Numerical Model
The aerodynamic problem is solved using the Unsteady Vortex Lattice Method, modelling lifting surfaces through discretised vortex lattices and wake evolution in time.

Time-marching simulations capture wake deformation and unsteady aerodynamic loading.

### Rotating Blade Modelling
The original implementation was adapted to support rotating lifting surfaces.  
This required modifications to the handling of:

- time-dependent geometry kinematics  
- wake convection for rotating blades 
- force coefficient extraction for rotor motion  

### Validation Approach
Computed aerodynamic coefficients were compared with benchmark reference data from the literature to assess agreement and model reliability.

---

## Analyses and Results

### Two-Blade Rotor in Hover
The main results focus on a two-blade rotor configuration operating in hover conditions.

The following parametric studies were performed:

#### Effect of Blade Angle of Attack (Hover, zero vertical velocity)
Thrust coefficient variation vs blade rotation angle was analysed for two angles of attack:
- 5°
- 8°

#### Effect of Vertical Freestream Velocity
For a fixed blade angle of attack (5°), simulations were performed with multiple non-zero vertical freestream velocities to evaluate their effect on thrust generation.

---

## Figures
The reported figures show selected results and comparisons between computed results and benchmark reference data.

They include:

- thrust coefficient vs blade rotation angle
- influence of the blade angle of attack
- influence of vertical freestream velocity
- agreement with benchmark solution

(Additional benchmark configurations were simulated and may be documented in future updates.)

---

## Tools and Technical Concepts
- Unsteady Vortex Lattice Method (UVLM)
- Time-marching wake modelling
- Rotor aerodynamics
- Numerical simulation and validation against benchmark data
- Python-based computational analysis

---

## Code Availability
Simulations were performed using an academic UVLM implementation developed within a university research environment and adapted by the author for rotating blade applications.

The full source code cannot be publicly distributed.  
However, methodological details and results are presented for portfolio and demonstration purposes.  
Additional information may be provided upon request.

---
