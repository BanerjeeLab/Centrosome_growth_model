# Centrosome_growth_model
This repository contains the codes used to study size regulation of centrosomes during centrosome maturation before cell division. Please see the corresponding [publication](https://duckduckgo.com) for more information. We used these codes to simulate stochastic growth of centrosomes in a cell with finite amount of building blocks. It includes codes for the different models used such as autocatalytic and catalytic growth etc as we describe below.  

**Some background information**
* The codes are written in FORTRAN90 and compiled and used in a linux environment.
* We use [Gillespie's first algorithm](https://pubs.acs.org/doi/10.1021/j100540a008) to evluate the stochastic trajectories based on the corresponding chemical master equations.
* To simulate diffusion, we have modelled it as a reaction based on the [work of D. Bernstein](https://doi.org/10.1103/PhysRevE.71.041103).
* Unless mentioned specifically, the codes simulate growth of two centrosomes.

**Prerequisites**
* G-fortran software
* A repository named "data" where the output files will be written

**Output data**
* In the code "autocatalytic_growth.f90" the output file "l.txt" contains four columns : `t,l1*dv,l2*dv,m` which denote time (in sec), volume of the first centrosome (in micro-meter cube), volume of the second centrosome (in micro-meter cube), building blocks in the cytoplasmic pool.
* In the code "catalytic_growth.f90" the output file "l.txt" contains four columns : `t,(l1)*dv,(l2)*dv,m,ms,le,me` which denote time (in sec), volume of the first centrosome (in micro-meter cube), volume of the second centrosome (in micro-meter cube), inactive subunits in the cytoplasmic pool, active subunits in the cytoplasmic pool, active enzymes in the cytoplasmic pool, inactive enzymes in the cytoplasmic pool.



[1]: [https://pubs.acs.org/doi/10.1021/j100540a008] 'T.D. Gillespie, Exact stochastic simulation of coupled chemical reactions, J Chem. Phys., 1977'
[2]: [https://doi.org/10.1103/PhysRevE.71.041103] 'D. Bernstein, Simulating mesoscopic reaction-diffusion systems using the Gillespie algorithm, Phys. Rev. E, 2005'

