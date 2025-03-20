---
layout: post

title: a post with formatting and links
description: march & april, looking forward to summer
thumbnail: assets/img/9.jpg
date: 2025/03/20 19:10:53
 # in terminal: Get-Date -Format "yyyy/MM/dd HH:mm:ss" ;

tags: formatting links
categories: sample-posts

related_projects: []

giscus_comments: true

featured: false
---

# Reconstructing Cortical Activity from MEG: Exploring Source Models and Frequency Bands

> The text in this blogpost has been produced partly by ChatGPT-4o.

Magnetoencephalography (MEG) provides exquisite temporal resolution to monitor the brain's electromagnetic activity non-invasively. However, the challenge lies in solving the *inverse problem*—inferring the location and strength of the underlying neural sources that generate the magnetic fields detected outside the head. Several mathematical approaches have been developed for this task, each imposing distinct assumptions and priors about the brain’s activity. In this post, I’ll walk you through videos of cortical reconstructions using four widely used methods: **Minimum Norm Estimate (MNE)**, **dynamic Statistical Parametric Mapping (dSPM)**, **sLORETA**, and **LCMV Beamforming**.

Before diving into these methods, it is essential to understand the distinction between the *forward* and *inverse* problems in MEG.

## The Forward Model: A Well-Posed Problem

The forward model mathematically describes how neural currents in the brain generate magnetic fields measurable by MEG sensors. This is a well-posed problem: given a known distribution of sources, one can compute the sensor-level magnetic fields uniquely and stably using Maxwell's equations and a model of the head's conductivity. The relationship is linear:
$$
\mathbf{B} = \mathbf{G} \mathbf{J} + \mathbf{N}
$$

where:

- $\mathbf{B}$ is the measured sensor data,
- $\mathbf{G}$ is the lead field matrix (forward model),
- $\mathbf{J}$ is the source current distribution,
- $\mathbf{N}$ represents measurement noise.

The lead field matrix $\mathbf{G}$ encapsulates how each unit dipole at each cortical location contributes to the magnetic field at each sensor, considering the head's geometry and conductivity. This matrix is critical for solving the inverse problem.

## The Inverse Problem: Ill-Posed by Nature

In contrast, the inverse problem aims to estimate $\mathbf{J}$ given $\mathbf{B}$ and $\mathbf{G}$. This problem is ill-posed because there are infinitely many possible source configurations that can produce the same external magnetic field. Furthermore, MEG is primarily sensitive to tangential sources, adding another layer of ambiguity.

To make the inverse problem solvable, all source reconstruction methods rely on additional constraints or priors (e.g., minimizing current norms, applying statistical normalization, or enforcing spatial smoothness). The forward model $\mathbf{G}$ is the cornerstone for computing the inverse solutions, connecting the physiological assumptions to the measured data.

## The Mathematics of Source Reconstruction

### Minimum Norm Estimate (MNE)

MNE solves the inverse problem by minimizing the norm of the current distribution:

$\hat{\mathbf{J}} = \mathbf{G}^\top (\mathbf{G} \mathbf{G}^\top + \lambda \mathbf{C})^{-1} \mathbf{B}$

where:

- $\mathbf{B}$ is the sensor data,
- $\mathbf{G}$ is the lead field matrix,
- $\lambda$ is the regularization parameter,
- $\mathbf{C}$ is the noise covariance matrix.

The solution favors low-amplitude distributed sources and is inherently biased toward superficial currents due to depth attenuation.

### dynamic Statistical Parametric Mapping (dSPM)

dSPM builds on MNE by normalizing each estimated source by the local noise estimate:

$\text{dSPM} = \frac{\hat{\mathbf{J}}}{\sqrt{\mathrm{Var}(\hat{\mathbf{J}})}}$

This results in a z-score-like map, highlighting significant activations and reducing the influence of noise.

### sLORETA (Standardized Low Resolution Brain Electromagnetic Tomography)

sLORETA introduces an additional spatial smoothness constraint, estimating standardized currents by considering the Laplacian of the solution. This enhances depth localization while maintaining zero localization bias under ideal conditions.

#### LCMV Beamforming

The Linearly Constrained Minimum Variance (LCMV) beamformer spatially filters the data to maximize the signal from a target location while minimizing contributions from elsewhere:

$\mathbf{w} = \frac{\mathbf{C}^{-1} \mathbf{G}}{\mathbf{G}^\top \mathbf{C}^{-1} \mathbf{G}}$

LCMV assumes sources are uncorrelated and adapts dynamically to the data, making it sensitive to temporal structure but less robust to correlated sources.

------

## Constrained vs. Unconstrained Dipole Models

Source models can differ in how they treat the orientation of the equivalent current dipoles:

- **Constrained (Normal) Model:** Dipoles are fixed to be perpendicular to the cortical surface. This is physiologically plausible, as pyramidal neurons—primary generators of MEG signals—are oriented normal to the cortex. Constrained models reduce the dimensionality of the problem, enhance spatial resolution, and minimize spurious activations.
- **Unconstrained Model:** Dipoles are free to orient in three orthogonal directions at each source point. This increases model flexibility but at the cost of interpretability and susceptibility to noise, as non-physiological orientations may dominate in some regions.

In the first set of videos, you'll see the same brain activation reconstructed under both scenarios. Expect the unconstrained model to appear more "smeared" and complex, while the constrained model provides sharper, directionally meaningful activations.

<iframe width="560" height="515" src="https://www.youtube.com/embed/3sdBlywlENI?si=7ZwJxWo6PRUpJRep" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>





<iframe width="560" height="515" src="https://www.youtube.com/embed/1OVPjdXzoCY?si=Jkzg6D9DOSy4a0pb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>







------

## Oscillatory Bands: From Delta to Gamma

In the second part, I’ll show how these methods reveal activity within canonical brain rhythms by filtering the MEG data into five frequency bands:

| Band  | Frequency Range | Typical Function                       |
| ----- | --------------- | -------------------------------------- |
| Delta | 1–4 Hz          | Sleep, homeostasis, motivation         |
| Theta | 4–8 Hz          | Memory, navigation, cognitive control  |
| Alpha | 8–12 Hz         | Visual attention, idling state         |
| Beta  | 13–30 Hz        | Motor control, top-down processing     |
| Gamma | 30–100 Hz       | Perception, binding, active processing |

Filtering allows us to isolate the cortical dynamics associated with specific cognitive processes. For instance:

- **Alpha:** You might observe occipital alpha suppression during visual tasks (event-related desynchronization).
- **Beta:** Sensorimotor beta activity may reflect motor planning or inhibition.
- **Gamma:** High-frequency bursts can emerge during perception or attention, but be cautious—gamma is susceptible to muscle and eye movement artifacts.

Each band emphasizes different physiological mechanisms, and their cortical projections will look distinct—sometimes local, sometimes widespread—depending on the neural generators.



<iframe width="560" height="515" src="https://www.youtube.com/embed/ug0ArGkCnUI?si=_0VA00-aoHhcjsg4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>



<iframe width="560" height="515" src="https://www.youtube.com/embed/ug0ArGkCnUI?si=_0VA00-aoHhcjsg4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>



<iframe width="560" height="515" src="https://www.youtube.com/embed/rpnnFeuPyXs?si=AhTM4aSW5luORmpo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>



## Conclusion

By comparing these methods and models side by side, we’ll explore how different mathematical assumptions and biological constraints shape our interpretation of MEG data. This exercise not only helps us appreciate the complexity of source modeling but also provides insights into brain rhythms and their functional significance.