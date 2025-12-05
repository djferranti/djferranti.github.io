---
title: Research
layout: single
classes: wide
permalink: /research/
author_profile: true
---
## Academic work
### In Review/Preprints
[*Analysis of the stability of an immersed elastic surface using the method of regularized Stokeslets*](https://arxiv.org/abs/2507.07063v1), **DF**, S.D. Olson. *Accepted by JCP pending review of minor revisions.* 
### Peer-reviewed
[*Regularized Stokeslet Surfaces*](https://www.sciencedirect.com/science/article/pii/S0021999124002535), **DF**, R. Cortez. *Journal of Computational Physics*, 2024.

[Correction]({{ site.baseurl }}/assets/manuscripts/erratum.pdf) \
[Matlab Code Github Repository](https://github.com/djferranti/RegularizedStokesletSurfaces)

[Python Code Github Repository](https://github.com/djferranti/RegularizedStokesletsTutorial/tree/main/reg_stokeslet_surfaces)

### Dissertation
[*Regularized Stokeslet Surfaces and a Coupled Oscillator System in Stokes Flow*](https://digitallibrary.tulane.edu/islandora/object/tulane%3A144133)

### Older work
[*Generalized matching preclusion in bipartite graphs*](https://digitalcommons.georgiasouthern.edu/tag/vol5/iss1/1/), *Theory and Applications of Graphs*, 2018.

[*The value of prior knowledge in machine learning of complex network systems*](https://pubmed.ncbi.nlm.nih.gov/29036404/), **DF**, D. Krane, D. Kraft. *Bioinformatics*, 2017.

## Numerical methods for Stokes flow
In a number of interesting biological and physical applications, viscous forces are several orders of magnitude greater than inertial forces. For these situations, modelers use the Stokes equations to describe the fluid dynamics. In applications, one has a fluid-structure interaction problem where the structure (e.g. solid boundary, active flagellum/cilium) exerts forces on the fluid. These problems are often nontrivial due to complex geometries, moving, and the nonlinear coupling between the structures and the fluid. While a number of methods are available for numerical simulations of these problems, I have devoted most of my research to the method of regularized Stokeslets (MRS). Two of these projects are described below.

### Stability Analysis of an Elastic Surface with the MRS
We examined the linearized stability of a perturbed elastic surface in a Stokes fluid using the MRS. By formulating the problem in a doubly periodic domain, we used Fourier techniques to analyze the spectrum of the system. The analysis revealed the effect of the choice of regularization function, parameters, and constitutive model for the elastic surface on the critical time step necessary to ensure stability. 

### Regularized Stokeslet Surfaces
Regularized Stokeslet surfaces are an extension to the MRS which utilizes exact integration over a triangulated surface. Effectively, the spatial discretization of the boundary is numerically "decoupled" from the choice of regularization parameter. In the typical implementation of the MRS, these parameters are always chosen in tandem: if the regularization is too small relative to the spatial discretization, the fluid velocity is not evaluated accurately near the boundary and fluid "leaks through." This method allows one to use fewer points to discretize a boundary and evaluate the nearly singular integrals accurately near the boundary. 

## Coupled oscillators in Stokes flows
In my thesis, I worked on the analysis of a coupled oscillator model in Stokes flow. The oscillators were spheres which moved due to an external forcing from a spring-like system. The motion of the oscillators was coupled through the fluid. We showed that the in-phase state can be stabilized through the introduction of either an additional elastic coupling between the oscillators, or "weak inertia" which is effected by modeling the fluid with the unsteady Stokes equations. I am currently working with an undergraduate student on new questions involving this model.

## Jupyter Notebooks on MRS
For a tutorial I helped run at a workshop in July 2025, I made two Jupyter notebooks which are now hosted on Github:

* [Moment Conditions Jupyter Notebook](https://github.com/djferranti/RegularizedStokesletsTutorial/blob/main/moments.ipynb)
* [Regularized Stokeslet Surfaces Notebook](https://github.com/djferranti/RegularizedStokesletsTutorial/blob/main/flow_past_sphere_streamlines.ipynb)

The first notebook is self-contained and shows how using blobs with particular moment conditions increases the convergence of the far-field regularization error.

The second notebook requires the Python version of the regularized Stokeslet surfaces code, also [on Github](https://github.com/djferranti/RegularizedStokesletsTutorial/tree/main/reg_stokeslet_surfaces). The first few cells are not necessary if you have the required dependencies and are running locally (not in Google CoLab). 
