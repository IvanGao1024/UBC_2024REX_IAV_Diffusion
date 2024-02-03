# REX_IAV_Diffusion_Simulation

This is the repo for the University of British Columbia Undergraduate Research Experience Program Math Bio Group 2023-11 to 2024-03. The code is developed in Julia where the math parameters are chosen from Vahey and Fletcher's paper. [1]

## Research question: Simulation of influenza A virus (IAV) mobility under different ligand organization

## Pkg used
using Plots
using LinearAlgebra
using Random
using Luxor

## General Ligand Setup
![IAV_orgnization](img/AxisSetup.png)[1]

# Assumptions: P1 is SA carpet, P2 is anti-body suspension, P3 is horizontal plane of IAV
1. Dist(P1, P2, P3) are neglected. P1, P2, P3 are suppose to be 3D but height dimention got removed due to 2D simulation restriction. So consider them as projection to plane
2. Cleaved SA are super weak to futher bind so get removed from simulation


# TODO:
- Fix the problem that the output anim or gif isn't moving.
- movement function with binding restriction
- Make IAV organization more controllable by allowing patterns like mixing regions and randomly deactivating HA/NA ligands. 

Bibliography:
[1] M. D. Vahey and D. A. Fletcher, “Influenza A virus surface proteins are organized to help penetrate host mucus,” eLife, vol. 8, p. e43764, May 2019, doi: 10.7554/eLife.43764.
=#