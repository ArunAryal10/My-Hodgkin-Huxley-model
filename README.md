# Hodgkin–Huxley Neuron Model (MATLAB)

![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?logo=mathworks&logoColor=white)
![Computational Neuroscience](https://img.shields.io/badge/Computational-Neuroscience-8A2BE2)

A from-scratch MATLAB implementation of the classic **Hodgkin–Huxley model** — the biophysical model of the neuronal action potential that earned Hodgkin and Huxley the 1963 Nobel Prize.

## What it models

The membrane potential is driven by four coupled dynamical variables:

- **V** — membrane potential
- **m** — sodium-channel activation gate
- **h** — sodium-channel inactivation gate
- **n** — potassium-channel activation gate

Their interplay across voltage-gated Na⁺ and K⁺ conductances (plus a leak current) generates the characteristic spike. The model uses standard steady-state activation functions (`m_inf`, `h_inf`, `n_inf`) and voltage-dependent time constants, integrated numerically over time with an applied current step.

## Parameters (as implemented)

Membrane capacitance `C = 1`; reversal potentials `E_Na = 55`, `E_K = -75`, `E_L = -52`; maximal conductances `g_Na = 120`, `g_K = 36`, `g_L = 0.3`; time step `dt = 0.01` ms over a 5,000 ms simulation with a current step applied mid-trial.

## Run it

Open `MY_HODGHUX.m` in MATLAB and run — it simulates the membrane potential over time and plots the resulting action-potential train.

## Tech stack

MATLAB (no toolboxes required)
