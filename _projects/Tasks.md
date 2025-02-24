---
layout: project
title: Cognitive Tasks
description: >
  modeling brain activity in cognitive tasks through whole-brain simulations

importance: 5
category: research

related_publications: false
related_blog_posts: true
---


Most whole-brain modeling research has focused on replicating brain activity in the resting state. While this approach
has led to significant insights into large-scale network dynamics, cognitive function emerges from active, task-driven
states. Bridging the gap between brain modeling and cognitive modeling presents an opportunity to enhance both fields,
integrating mechanistic explanations of neural dynamics with functional accounts of cognition.

#### The Challenge: From Resting-State to Task-Based Modeling

Whole-brain models typically simulate the spontaneous activity of large-scale networks, often constrained by structural
connectivity from diffusion MRI. While these models capture key resting-state features, including functional
connectivity dynamics, their application to cognitive processes remains limited. Cognitive states involve transient,
task-specific activations, recruiting distinct brain networks depending on the task demands. A crucial step forward is
the incorporation of task-driven constraints into whole-brain models to explore how neuronal populations coordinate
during cognitive processes.

#### Cognitive Models: The Role of ACT-R

One of the most influential frameworks in cognitive modeling is the **Adaptive Control of Thought—Rational (ACT-R)**
architecture. ACT-R is a computational cognitive architecture designed to simulate human thought processes. It is based
on a modular structure where different components correspond to distinct cognitive functions, such as memory retrieval,
perceptual processing, and motor execution. These modules communicate through a central procedural system, which selects
rules for action based on environmental stimuli and internal goals.

ACT-R has been used extensively in psychology and artificial intelligence to model problem-solving, learning, and
decision-making processes. Its symbolic and subsymbolic mechanisms allow it to represent both high-level cognitive
functions (e.g., language processing) and more fine-grained adaptations based on experience. While ACT-R provides a
robust framework for simulating cognition, its connection to the neurobiological substrate remains an open challenge.

#### Towards a Unified Framework: Linking Brain Activity Models with Cognitive Models

To advance cognitive neuroscience, we need to bridge the gap between models of brain dynamics and cognitive
architectures like ACT-R. A promising approach is to constrain whole-brain simulations with task-based empirical data,
ensuring that the simulated neural activity reflects cognitive task execution. Several strategies could facilitate this
integration:

- Task-Evoked Connectivity: Incorporating experimental data from task-based fMRI or MEG studies to modulate network
  interactions dynamically.
- Neurophysiological Constraints: Embedding neurophysiological principles (e.g., neural adaptation, synaptic plasticity)
  into cognitive models to generate biologically plausible outputs.
- Hybrid Models: Combining symbolic cognitive architectures (like ACT-R) with neural mass models or spiking network
  models to simulate cognitive processes at multiple levels of abstraction.
- Predictive Validation: Using cognitive models to generate testable predictions about brain activity, which can be
  compared against empirical neuroimaging or electrophysiological data.

#### Future Directions and Applications

Integrating whole-brain modeling with cognitive modeling has profound implications for understanding cognition and its
disorders. This approach could help decode how large-scale brain networks adapt to different cognitive demands, shedding
light on individual differences in problem-solving and decision-making. Moreover, it offers a potential framework for
studying cognitive dysfunction in neurological and psychiatric conditions, where deviations from normative brain
dynamics impact cognitive performance.

By leveraging insights from both neuroscience and cognitive science, we can move toward a more comprehensive
understanding of how the brain supports intelligent behavior, ultimately refining our ability to model and predict
cognitive processes in real-world scenarios.