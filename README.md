# Brownian-Langevin simulation and evanescent wave dynamic light scattering
---
This is a simulation of near wall diffusion and flow as seen by the experimental technique of evanescent wave dynamic light scattering (EW-DLS) [[2-4]](#2).

You can demo the simulation online through the link below but it is recommended that you download it onto your computer as it will run faster.  

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/antgi1/bd_demo/master?filepath=bd_simu.ipynb)


## Simulation
The code here is as described in [[4]](#4). 
The simulation box is in 2 dimensions with cyclic boundary conditions in the x axis and reflection at both boundaries perpendicular to the z-axis. Motion of the particles is over damped, meaning there is no inertia. No interactions are considered between the particles. Length units are set according to the particle radius.



## DLS
DLS (also known as photon correlation spectroscopy, PCS) is a technique routinely used to characterize small particles such as polymers and colloids [[1]](#1). 

A laser beam is used to probe the sample and the measured quantity in the experiment is the sum (interference) of the scattered light by all of the particles in the scattering volume. The intensity auto-correlation, <I(t)*I(t+tau)>/<I(t)^2>, is calculated and from there the diffusion coefficient (proportional to a hydrodynamic radius) of the particles in a medium is calculated. The auto-correlatin function can be measured in real time thanks to multiple-tau correlators. Through careful measurement and modeling other information such as internal structure and interactions can be recovered.

## EW-DLS
EW-DLS is variation of the technique where a total internal reflection evanescent field is used to probe dynamics within one wavelength of light (~500 nm) of an interface [[2]](#2). From the localization of the probe results that effects due to interactions of the particles with the wall can be measured.

### Velocimetry
EW-DLS can be used to measure flow with very strong near wall sensitivity [[3-4]](#3). This is potentially useful for the study of dynamic interactions between a complex fluid and the wall. An example of this is the characterization of the boundary condition at the interface with the solid wall (mainly the presence of slip and its quantification [[4-5]](#4)).

## Multiple tau correlator
Dynamics in soft materials can vary over several decades in time. DLS traditionally makes use of the multiple-tau correlator that allows calculation of a correlation function over a wide range of time with limited resources. Its working principle is the calculation of the correlation at points spread almost linearly in a logarithmic scale. 

The correlator used here was adapted from the code by J. Ramírez [[6]](#6).

[1] <a name="1">https://en.wikipedia.org/wiki/Dynamic_light_scattering </a>  
[2] Light scattering near and from interfaces using evanescent wave and ellipsometric light scattering <a name="2">https://doi.org/10.1016/j.cocis.2009.08.004</a>  
[3] Near-field laser Doppler velocimetry measures near-wall velocities <a name="3">https://doi.org/10.1140/epje/i2012-12062-5  </a>  
[4] Near wall velocimetry on a rheometer <a name="4">https://doi.org/10.1122/1.5047020   </a>  
[5] https://en.wikipedia.org/wiki/No-slip_condition  <a name="5">https://en.wikipedia.org/wiki/Dynamic_light_scattering </a>  
[6] https://en.wikipedia.org/wiki/No-slip_condition  <a name="6">[6] https://doi.org/10.1063/1.3491098 </a>
