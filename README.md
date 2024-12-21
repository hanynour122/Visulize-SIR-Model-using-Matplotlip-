## Project Discussion

This repository implements the SIR (Susceptible-Infected-Recovered) model using the Runge-Kutta method for solving differential equations. The model simulates the spread of infectious diseases within a population and provides valuable insights into the dynamics of an outbreak.

### Purpose
The purpose of this project is to model the spread of infectious diseases using the SIR model and analyze how the disease evolves over time. By using numerical methods such as the Runge-Kutta method, we can more accurately predict the future course of the disease compared to simpler methods like Euler’s method. 

**Understanding how diseases spread and recover can inform strategies for prevention and intervention, such as vaccination programs or quarantine measures.**

### Key Components:
- **SIR Model:** Describes the transitions between three states of individuals: Susceptible (S), Infected (I), and Recovered (R).
- **Runge-Kutta Method:** A more accurate method for numerically solving ordinary differential equations compared to simpler approaches.
- **Simulation:** The model simulates disease dynamics over time, generating outputs such as the number of susceptible, infected, and recovered individuals at each timestep.

## Model Equations
The following differential equations represent the basic SIR model:

1. **dS/dt = -beta * S * I / population**
   - Susceptible individuals transition to infected as they come into contact with infected individuals.

2. **dI/dt = beta * S * I / population - gamma * I**
   - Infected individuals either recover or continue spreading the disease.

3. **dR/dt = gamma * I**
   - Recovered individuals are no longer susceptible and are considered immune.

Where:
- **beta** is the transmission rate.
- **gamma** is the recovery rate.
- **population** is the total number of individuals in the system.

**The Runge-Kutta method is used to solve these equations over time, with intermediate steps (k1, k2, k3, k4) helping to approximate the solution.**

