# Wildfire Risk: Stochastic Optimisation & Simulation

Optimising firebreak placement under budget constraints and evaluating outcomes under uncertainty, combining mathematical optimisation with Monte Carlo simulation and tail-risk analysis.

## Overview

Wildfire mitigation involves deciding where to place limited resources (firebreaks) to reduce potential damage, under both budget limits and genuine uncertainty about how fires spread. This project modelled that as an optimisation problem and then stress-tested the chosen strategies under stochastic conditions to understand not just expected outcomes, but worst-case (tail) risk.

## Approach

- **Optimisation:** formulated a max-flow network model and two mixed-integer linear programming (MILP) formulations to optimise firebreak placement under budget constraints, implemented in AMPL/Gurobi.
- **Simulation:** built Monte Carlo simulations in R (N = 1000) with custom samplers to evaluate outcomes under stochastic fire-spread conditions.
- **Risk analysis:** computed CVaR (Conditional Value at Risk) alongside expected damage to capture tail risk in right-skewed outcome distributions, reported with 95% confidence intervals.

## Results

- Produced optimised firebreak placement strategies within budget constraints.
- Quantified not only expected damage but tail-risk exposure, giving a fuller picture of how strategies perform under worst-case scenarios rather than on averages alone.

## Tools & Techniques

`R` · `AMPL` · `Gurobi` · mixed-integer linear programming (MILP) · max-flow network modelling · Monte Carlo simulation · CVaR / tail-risk analysis · confidence intervals

## What I learned

- Translating a real-world resource-allocation problem into rigorous optimisation formulations.
- Combining optimisation with simulation to test solutions under uncertainty rather than assuming fixed conditions.
- Quantifying tail risk (CVaR) — directly relevant to risk modelling in finance and beyond.

## Notes

Completed as part of my degree at LSE. This repository documents the methodology and results; shared or third-party data is described rather than redistributed.
