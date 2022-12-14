---
layout: page
title: "Schrödinger"
permalink: /QM
---

# Schrödinger's equation simulations

Python simulation of both time-dependent and time independent Schrödinger equation (TDSE and TIDSE respectively).<br /><br />
The wave function of a particle squared determines it's probability density of its position. The reason it is called a **wave**function is due to it being a **complex** function, which gives it its wave properties (due to the [complex exponential](https://en.wikipedia.org/wiki/Euler%27s_formula)).
## The time-dependent Schrödinger equation ([TDSE](https://en.wikipedia.org/wiki/Schr%C3%B6dinger_equation#Time-dependent_equation))
<img src="https://wikimedia.org/api/rest_v1/media/math/render/svg/4e59451da64dff4be22db56d1adf9968e2a32d9c" width=50% height=50%><br />
The time-dependent Schrödinger equation is a second order linear partial differential equation that governs the evolution of the wave function of a quantum-mechanical system.<br /> 

## The time independent Schrödinger equation ([TIDSE](https://en.wikipedia.org/wiki/Schr%C3%B6dinger_equation#Time-independent_equation))
<img src="https://wikimedia.org/api/rest_v1/media/math/render/svg/d6ce1cc8ef9ec26c68c7ba654a371194e41a316f" width=40%><br />
However, the time-independent Schrödinger equation describes stationary states, which are eigenfunctions of the Hamiltonian. The stationary state's probability density are constant in time, but a superposition of these states are not stationary. The TIDSE can help simplify the solving of the TDSE.<br />

## General solution of TDSE
<img src="https://latex.codecogs.com/svg.image?\huge&space;\mathcal{T}\exp(&space;-\frac{i}{\hbar}&space;\int_{t_{0}}^{t}&space;\hat{H}(\tau)\mathrm{d}\tau)&space;" width=50%><br />
The algorithm used for TDSE is [A fast explicit algorithm for the time-dependent Schrödinger equation](https://aip.scitation.org/doi/abs/10.1063/1.168415) by Pieter B. Visscher, which uses the [leapfrog integrator](https://en.wikipedia.org/wiki/Leapfrog_integration) to integrate the equations.
