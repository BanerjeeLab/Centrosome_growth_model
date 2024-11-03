# Centrosome_growth_model
This repository contains the codes used to study size regulation of centrosomes during centrosome maturation before cell division. Please see the corresponding [publication](https://duckduckgo.com) for more information. We used these codes to simulate stochastic growth of centrosomes in a cell with finite amount of building blocks. It includes codes for the different models used such as autocatalytic and catalytic growth etc as we describe below.  

**Some background information**
* The codes are written in FORTRAN90 and compiled and used in a linux environment.
* We use [Gillespie's first algorithm](https://pubs.acs.org/doi/10.1021/j100540a008) to evluate the stochastic trajectories based on the corresponding chemical master equations.
* To simulate diffusion, we have modelled it as a reaction based on the [work of D. Bernstein](https://doi.org/10.1103/PhysRevE.71.041103).






[1]: [https://pubs.acs.org/doi/10.1021/j100540a008] 'T.D. Gillespie, Exact stochastic simulation of coupled chemical reactions, J Chem. Phys., 1977'
[2]: [https://doi.org/10.1103/PhysRevE.71.041103] 'D. Bernstein, Simulating mesoscopic reaction-diffusion systems using the Gillespie algorithm, Phys. Rev. E, 2005'

