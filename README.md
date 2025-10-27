# Power-Dispatch-Optimization
A minimal, transparent **energy-system optimization** model built with [PuLP](https://github.com/coin-or/pulp).  
It reproduces merit-order dispatch and inter-regional power flows in a 3-node power system (North–Central–South).

## 🧠 What It Does
- Minimizes total system generation cost.
- Respects plant capacity limits and inter-regional transmission capacities.
- Demonstrates **how cheap baseload in one region displaces expensive peakers elsewhere**.
- Outputs generation mix, power flows, and regional balances.

## 🗺️ Model Structure
| Element | Meaning |
|:--|:--|
| **Regions** | North, Central, South |
| **Technologies** | Wind, Nuclear, Biomass, Coal, Gas |
| **Decision variables** | Generation per plant, power flow per corridor |
| **Objective** | Minimize total generation cost (€/h) |
| **Constraints** | Plant capacities, nodal balance, line capacities |
