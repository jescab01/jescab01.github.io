---
layout: project
title: transcraneal Stimulation
description: >
  modeling the effects on brain tissue, 
   from current propagation to network-level modulation and cognitive applications.

img: assets/img/2.jpg
importance: 3
category: research

related_publications: true
related_blog_posts: true
---

#### Understanding Non-Invasive Brain Stimulation (NIBS)

Non-invasive brain stimulation (NIBS) techniques, such as transcranial electrical stimulation (tES), provide a means to
modulate brain activity using weak electrical currents applied to the scalp. Among these, transcranial alternating
current stimulation (tACS) and transcranial direct current stimulation (tDCS) are widely studied for their ability to
influence neuronal excitability and network function. These techniques hold potential for both fundamental neuroscience
and clinical interventions, but their effects must be carefully modeled to maximize efficacy and specificity.

#### Modeling Current Propagation: From Electrodes to the Brain

To understand and optimize the effects of transcranial stimulation, it is crucial to model how electrical currents
propagate through biological tissues. This involves simulating how electrical fields travel through the skin, skull,
cerebrospinal fluid, and brain tissue, taking into account the varying conductivity of each layer. Using MRI-based
reconstructions of individual head anatomy, realistic models can predict the spatial distribution of electric fields and
their interaction with cortical and subcortical structures. These simulations provide insight into the effectiveness and
precision of stimulation protocols and help refine experimental and clinical applications.

#### Taking Cortical Geometry Into Account

The brain's folded structure significantly influences how electric fields interact with neuronal populations. Advanced
modeling techniques integrate realistic cortical geometry to:

- Identify areas where stimulation is most effective.
- Assess differences in electric field strength across gyral and sulcal surfaces.
- Improve accuracy in predicting neuronal responses to stimulation.

> Related citations {% cite Cabrera-Alvarez2023-tACS %}

#### Optimizing Electrode Montages for Targeted Stimulation

The placement of stimulation electrodes is a critical factor in determining both the focality and effectiveness of
neuromodulation. Computational modeling enables the optimization of electrode configurations by identifying montages
that maximize the desired effect while minimizing unintended stimulation of surrounding regions. Subject-specific models
further enhance this approach, allowing stimulation parameters to be tailored to individual anatomical differences. This
personalized strategy is particularly relevant for clinical applications where precision is key.

#### Linking Electric Field Effects to Brain Activity

While current propagation models provide a detailed view of where stimulation reaches, understanding how it interacts
with brain activity requires linking these models to neural dynamics. Electric fields influence neuronal excitability,
but their effects are state-dependent, meaning they interact with ongoing brain activity in complex ways. This research
aims to explore how externally applied stimulation modulates endogenous oscillations, alters functional connectivity,
and reshapes large-scale network activity. Integrating electric field modeling with computational brain activity
simulations provides a more complete framework for predicting stimulation outcomes.

#### Towards Functional and Clinical Applications

Beyond understanding the mechanisms of tES, a key goal is to leverage stimulation to target specific network disruptions
and cognitive processes. Future research directions include:

- Restoring Network Function: Using stimulation to counteract maladaptive network activity in neurological and
  psychiatric conditions.

- Enhancing Cognition: Exploring the use of tACS and tDCS to modulate cognitive functions such as attention, memory, and
  learning.
- Closed-Loop Stimulation: Developing adaptive stimulation protocols that respond dynamically to brain activity in real
  time.

This research line aims to bridge biophysical modeling, neurophysiology, and cognitive neuroscience to refine and
optimize the use of transcranial stimulation as both an investigative and therapeutic tool.