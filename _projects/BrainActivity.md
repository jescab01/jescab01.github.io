---
layout: project
title: Brain activity
description: >
  computational models of brain activity,
  from neural mass dynamics to whole-brain network simulations,
  to better understand large-scale brain function.

img: assets/img/1.jpg
importance: 1
category: research

related_publications: true
related_blog_posts: true
---

#### Understanding the Principles of Brain Simulation

Brain activity emerges from the complex interplay of neural populations and their structural connections. Computational
models allow us to simulate these dynamics, providing insights into how different regions interact and how large-scale
brain function arises from local neural mechanisms. This research line explores how to construct and refine such models
to better capture real brain activity.

#### Neural Mass Models: Simulating Local Population Dynamics

Neural mass models serve as a mathematical framework for approximating the collective activity of large groups of
neurons. By adjusting their parameters, we can reproduce different oscillatory behaviors observed in
electrophysiological recordings. Exploring these models helps us understand how local circuit dynamics contribute to
overall brain function and dysfunction.

#### Structural Constraints: Extracting Connectivity from dMRI

Long-range communication between neural populations is constrained by the brain’s structural connectivity.
Diffusion-weighted MRI (dMRI) provides a means to reconstruct white matter pathways and quantify connectivity strength
between regions. By integrating these structural features into computational models, we can simulate biologically
plausible network interactions and study their role in shaping brain activity.

#### Brain Network Models: Merging Dynamics and Structure

Combining neural mass models with structural connectivity data leads to brain network models—simulations that capture
how distributed regions interact dynamically. These models provide a powerful tool to investigate large-scale functional
connectivity, spectral properties, and topographical organization, helping bridge the gap between structural and
functional neuroimaging findings.

#### Parameter Exploration: Matching Models to Real Brain Activity

Brain network models must be carefully parameterized to reproduce empirical observations. Key aspects include:

- Spectral properties: Matching frequency-specific activity patterns seen in MEG/EEG data.
- Topographical organization: Ensuring spatial correspondence between simulated and real activation maps.
- Functional connectivity: Reproducing the network interactions observed in resting-state and task-based
  neuroimaging.
  By systematically tuning model parameters, we aim to generate simulations that align closely with empirical brain
  dynamics.

> Related citations {% cite Cabrera-Alvarez2023-Thalamus %}


#### Future Directions: Expanding the Scope of Brain Simulations

As computational methods advance, several promising avenues for research emerge:

- Surface-Based Simulations: Moving beyond regional models to simulate activity directly on the cortical surface,
  capturing finer spatial details of brain function.
- Minimal Parcellations: Exploring ultra-fine-grained models where parcels are as small as individual mesh
  triangles, allowing for more precise representations of neural dynamics.

This research line contributes to the broader goal of developing biologically plausible and computationally efficient
models that enhance our understanding of brain function and its disruptions in neurological conditions.
