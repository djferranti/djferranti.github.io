---
title: Research
layout: single
classes: wide
permalink: /research/
author_profile: true
---
## Academic work
### In Review/Preprints
[*Analysis of the stability of an immersed elastic surface using the method of regularized Stokeslets*](https://arxiv.org/abs/2507.07063v1), **DF**, S.D. Olson.
### Peer-reviewed
[*Regularized Stokeslet Surfaces*](https://www.sciencedirect.com/science/article/pii/S0021999124002535), **DF**, R. Cortez. *Journal of Computational Physics*, 2024.

[Correction]({{ site.baseurl }}/assets/manuscripts/erratum.pdf) \
Code: see my [Github repository](https://github.com/djferranti/RegularizedStokesletSurfaces)

### Dissertation
[*Regularized Stokeslet Surfaces and a Coupled Oscillator System in Stokes Flow*](https://digitallibrary.tulane.edu/islandora/object/tulane%3A144133)

### Older work (as an undergraduate)
[*Generalized matching preclusion in bipartite graphs*](https://digitalcommons.georgiasouthern.edu/tag/vol5/iss1/1/), *Theory and Applications of Graphs*, 2018.

[*The value of prior knowledge in machine learning of complex network systems*](https://pubmed.ncbi.nlm.nih.gov/29036404/), **DF**, D. Krane, D. Kraft. *Bioinformatics*, 2017.

## Numerical methods for Stokes flow
In a number of interesting biological and physical applications, viscous forces are several orders of magnitude greater than inertial forces. For these situations, modelers use the Stokes equations to describe the fluid dynamics. In applications, one often has structures immersed in the fluid (e.g. solid boundaries, active flagella, cilia) which are coupled through the viscous hydrodynamics and the forces exerted by the structure on the fluid. While a number of methods are available for numerical simulations of these methods, I have devoted most of my research to the method of regularized Stokeslets (MRS). In particular, I have worked on two projects described below.


### Stability Analysis of an Elastic Surface with the MRS
We examined the linearized stability of a perturbed elastic surface in a Stokes fluid using the MRS. By formulating the problem in a doubly periodic domain, we used Fourier techniques to analyze the spectrum of the system. The analysis revealed the effect of the choice of regularization function, parameters, and constitutive model for the elastic surface on the critical time step necessary to ensure stability. 

### Regularized Stokeslet Surfaces
Regularized Stokeslet surfaces are an extension to the MRS which utilizes exact integration over a triangulated surface. Effectively, the spatial discretization of the boundary is numerically "decoupled" from the choice of regularization parameter. In the typical implementation of the MRS, these parameters are always chosen in tandem: if the regularization is too small relative to the spatial discretization, the fluid velocity is not evaluated accurately near the boundary and fluid "leaks through." This method allows one to use fewer points to discretize a boundary and evaluate the nearly singular integrals accurately near the boundary. 

## Coupled oscillators in Stokes flows
In my thesis, I worked on the analysis of a coupled oscillator model in Stokes flow. The oscillators were spheres which moved due to an external forcing from a spring-like system. The motion of the oscillators was coupled through the fluid. We showed that the in-phase state can be stabilized through the introduction of either an additional elastic coupling between the oscillators, or "weak inertia" which is effected by modeling the fluid with the unsteady Stokes equations. I am currently working with an undergraduate student on new questions involving this model.
