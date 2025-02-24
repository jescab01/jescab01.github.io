# Projects 

My research is centered on developing and applying computational models of brain function and its modulation to foster our understanding of mental health and disease, cognition and behaviour. While building and enhancing these computational models is a research endeavour on its own, their true value emerges when they are applied to address specific topics such as **Alzheimer’s disease** and **wellbeing**.

The diagram represents this interconnected framework. The **horizontal axis** represents the application domains—on one end, neurodegenerative conditions like **Alzheimer’s disease**, and on the other, broader aspects of **well-being**. The **vertical axis** reflects different modeling approaches, each contributing essential tools for investigating these topics:

- **Brain Activity Modeling** – Developing methods to characterize neural dynamics, which serve as a foundation for understanding cognitive processes and disease mechanisms.
- **Transcranial Stimulation Modeling** – Exploring how external interventions, such as non-invasive brain stimulation, interact with brain networks and influence cognition.
- **Cognitive Modeling** – Creating computational frameworks to simulate cognitive processes, providing insights into mechanisms underlying memory, decision-making, and learning.

Each of these modeling lines contributes independently to advancing neuroscience, but their **true power lies in their integration**. By refining fundamental methodologies, I aim to develop tools that can be applied across different domains, improving both our theoretical understanding and practical applications.

Beyond my academic research, I also engage in creative projects, including **music and poetry**, which, in their own way, reflect a complementary exploration of cognition and human expression.





## Research Projects



### Project - Alzheimer's disease

> subtitle: understanding functional connectivity changes in dementia



#### **Understanding Functional Connectivity in Neurodegeneration**

Alzheimer’s Disease (AD) is a progressive neurodegenerative disorder characterized not only by cognitive decline but also by widespread disruptions in brain network dynamics. Functional connectivity—how different brain regions communicate—evolves throughout the disease continuum, from preclinical stages to severe dementia. Understanding these changes is key to developing early biomarkers and intervention strategies.

#### **From Connectivity to Mechanisms: Computational Modeling of AD**

The human brain is a complex network, and its dysfunction in AD cannot be fully understood through isolated observations. Computational models allow us to explore how neurobiological alterations—such as synaptic dysfunction, neuronal loss, and network disconnection—contribute to the progressive breakdown of functional connectivity. These models provide a framework for linking neuroimaging findings with underlying neural mechanisms, offering a deeper insight into disease progression.

#### **The Role of Proteinopathy in Brain Dynamics**

A hallmark of AD is the accumulation of pathological proteins, such as beta-amyloid and tau, which spread across the brain in characteristic patterns. But how do these molecular changes translate into altered neuronal activity and network function? By integrating proteinopathy maps with computational modeling, we can investigate how these pathological processes shape functional connectivity and contribute to cognitive impairment.

#### **Bridging Scales: From Neurons to Whole-Brain Networks**

Alzheimer’s research requires a multiscale perspective, connecting microscopic cellular pathology with macroscopic brain dynamics. Cutting-edge techniques—ranging from large-scale brain simulations to multimodal neuroimaging—are helping to unravel how local molecular events cascade into system-wide dysfunction. This knowledge is essential for designing targeted interventions that go beyond symptom relief and tackle the fundamental mechanisms of neurodegeneration.

#### **Future Directions: Towards Personalized Models of AD Progression**

While group-level studies have provided valuable insights into AD progression, there is a growing need for personalized approaches. Could we predict an individual’s disease trajectory based on their unique brain network properties? How can computational models be leveraged to refine therapeutic strategies? The future of AD research lies in combining neuroimaging, computational modeling, and artificial intelligence to develop individualized disease predictions and interventions.



### Project - Brain activity

> subtitle: from neural mass dynamics to whole-brain network simulations, to better understand large-scale brain function

#### **Understanding the Principles of Brain Simulation**

Brain activity emerges from the complex interplay of neural populations and their structural connections. Computational models allow us to simulate these dynamics, providing insights into how different regions interact and how large-scale brain function arises from local neural mechanisms. This research line explores how to construct and refine such models to better capture real brain activity.

#### **Neural Mass Models: Simulating Local Population Dynamics**

Neural mass models serve as a mathematical framework for approximating the collective activity of large groups of neurons. By adjusting their parameters, we can reproduce different oscillatory behaviors observed in electrophysiological recordings. Exploring these models helps us understand how local circuit dynamics contribute to overall brain function and dysfunction.

#### **Structural Constraints: Extracting Connectivity from dMRI**

Long-range communication between neural populations is constrained by the brain’s structural connectivity. Diffusion-weighted MRI (dMRI) provides a means to reconstruct white matter pathways and quantify connectivity strength between regions. By integrating these structural features into computational models, we can simulate biologically plausible network interactions and study their role in shaping brain activity.

#### **Brain Network Models: Merging Dynamics and Structure**

Combining neural mass models with structural connectivity data leads to brain network models—simulations that capture how distributed regions interact dynamically. These models provide a powerful tool to investigate large-scale functional connectivity, spectral properties, and topographical organization, helping bridge the gap between structural and functional neuroimaging findings.

#### **Parameter Exploration: Matching Models to Real Brain Activity**

Brain network models must be carefully parameterized to reproduce empirical observations. Key aspects include:

- **Spectral properties**: Matching frequency-specific activity patterns seen in MEG/EEG data.
- **Topographical organization**: Ensuring spatial correspondence between simulated and real activation maps.
- **Functional connectivity**: Reproducing the network interactions observed in resting-state and task-based neuroimaging.
  By systematically tuning model parameters, we aim to generate simulations that align closely with empirical brain dynamics.

#### **Future Directions: Expanding the Scope of Brain Simulations**

As computational methods advance, several promising avenues for research emerge:

- **Surface-Based Simulations**: Moving beyond regional models to simulate activity directly on the cortical surface, capturing finer spatial details of brain function.
- **Minimal Parcellations**: Exploring ultra-fine-grained models where parcels are as small as individual mesh triangles, allowing for more precise representations of neural dynamics.

This research line contributes to the broader goal of developing biologically plausible and computationally efficient models that enhance our understanding of brain function and its disruptions in neurological conditions.





### Project - transcranial Stimulation

> subtitle: Modeling the effects of transcranial electrical stimulation on brain tissue, from current propagation to network-level modulation and cognitive applications.



#### Understanding Non-Invasive Brain Stimulation (NIBS)

Non-invasive brain stimulation (NIBS) techniques, such as transcranial electrical stimulation (tES), provide a means to modulate brain activity using weak electrical currents applied to the scalp. Among these, transcranial alternating current stimulation (tACS) and transcranial direct current stimulation (tDCS) are widely studied for their ability to influence neuronal excitability and network function. These techniques hold potential for both fundamental neuroscience and clinical interventions, but their effects must be carefully modeled to maximize efficacy and specificity.

#### Modeling Current Propagation: From Electrodes to the Brain

To understand and optimize the effects of transcranial stimulation, it is crucial to model how electrical currents propagate through biological tissues. This involves simulating how electrical fields travel through the skin, skull, cerebrospinal fluid, and brain tissue, taking into account the varying conductivity of each layer. Using MRI-based reconstructions of individual head anatomy, realistic models can predict the spatial distribution of electric fields and their interaction with cortical and subcortical structures. These simulations provide insight into the effectiveness and precision of stimulation protocols and help refine experimental and clinical applications.

#### Taking Cortical Geometry Into Account

The brain's folded structure significantly influences how electric fields interact with neuronal populations. Advanced modeling techniques integrate realistic cortical geometry to:

- Identify areas where stimulation is most effective.
- Assess differences in electric field strength across gyral and sulcal surfaces.
- Improve accuracy in predicting neuronal responses to stimulation.

#### Optimizing Electrode Montages for Targeted Stimulation

The placement of stimulation electrodes is a critical factor in determining both the focality and effectiveness of neuromodulation. Computational modeling enables the optimization of electrode configurations by identifying montages that maximize the desired effect while minimizing unintended stimulation of surrounding regions. Subject-specific models further enhance this approach, allowing stimulation parameters to be tailored to individual anatomical differences. This personalized strategy is particularly relevant for clinical applications where precision is key.

#### Linking Electric Field Effects to Brain Activity

While current propagation models provide a detailed view of where stimulation reaches, understanding how it interacts with brain activity requires linking these models to neural dynamics. Electric fields influence neuronal excitability, but their effects are state-dependent, meaning they interact with ongoing brain activity in complex ways. This research aims to explore how externally applied stimulation modulates endogenous oscillations, alters functional connectivity, and reshapes large-scale network activity. Integrating electric field modeling with computational brain activity simulations provides a more complete framework for predicting stimulation outcomes.

#### Towards Functional and Clinical Applications

Beyond understanding the mechanisms of tES, a key goal is to leverage stimulation to target specific network disruptions and cognitive processes. Future research directions include:

- Restoring Network Function: Using stimulation to counteract maladaptive network activity in neurological and psychiatric conditions.
- Enhancing Cognition: Exploring the use of tACS and tDCS to modulate cognitive functions such as attention, memory, and learning.
- Closed-Loop Stimulation: Developing adaptive stimulation protocols that respond dynamically to brain activity in real time.

This research line aims to bridge biophysical modeling, neurophysiology, and cognitive neuroscience to refine and optimize the use of transcranial stimulation as both an investigative and therapeutic tool.



### Project - Wellbeing

> subtitle: exploring the neural foundations of flow and presence for enhancing wellbeing

Wellbeing is a multifaceted concept that has been studied across psychology, neuroscience, and philosophy. From a neuroscientific perspective, understanding the neural correlates of wellbeing can help develop strategies to enhance mental and cognitive states. In this research line, I aim to explore wellbeing through electrophysiology and brain stimulation, focusing particularly on the experience of flow and presence.

#### Theoretical Framework: Seligman’s PERMA Model

One of the most comprehensive frameworks for wellbeing is Martin Seligman’s PERMA model. It posits that wellbeing is composed of five core elements:

1. Positive Emotions – The experience of pleasure, joy, and contentment.
2. Engagement – Deep involvement in activities, closely related to flow.
3. Relationships – Social connections and their impact on mental health.
4. Meaning – A sense of purpose and connection to something larger.
5. Accomplishment – Pursuing goals and achieving mastery.

While all five elements are crucial, my primary interest lies in **Engagement**, particularly in how neuroscience can elucidate the mechanisms underlying **flow states**.

#### Flow: The Neuroscience of Deep Engagement

Flow, as described by Mihály Csíkszentmihályi, is a state of deep absorption where an individual loses self-awareness and becomes fully engaged in an activity. This experience, often linked to intrinsic motivation, optimal performance, and a sense of effortlessness, has been associated with specific neural mechanisms. From a neuroscientific perspective, flow correlates with altered activity in the default mode network (DMN), leading to a decrease in self-referential processing, as well as enhanced connectivity in task-positive networks, which facilitates the coordination of attentional and sensorimotor systems. Additionally, changes in alpha and theta oscillations have been observed, with alpha synchronization in sensory regions and theta activity in prefrontal and midline structures. These electrophysiological markers make flow an intriguing phenomenon to study through resting-state EEG/MEG recordings and task-related neural activity.

#### Brain Stimulation as a Tool to Modulate Flow and Presence

Transcranial electrical stimulation (tES), including transcranial alternating current stimulation (tACS) and transcranial direct current stimulation (tDCS), provides a potential avenue for enhancing or modulating flow and presence. By integrating electrophysiological recordings with brain stimulation, this research could contribute to developing non-invasive interventions aimed at optimizing cognitive and emotional states associated with wellbeing.

#### Future Directions

This research line is under construction.





### Project - Cognitive tasks

> subtitle: ¿?

Most whole-brain modeling research has focused on replicating brain activity in the resting state. While this approach has led to significant insights into large-scale network dynamics, cognitive function emerges from active, task-driven states. Bridging the gap between brain modeling and cognitive modeling presents an opportunity to enhance both fields, integrating mechanistic explanations of neural dynamics with functional accounts of cognition.

#### The Challenge: From Resting-State to Task-Based Modeling

Whole-brain models typically simulate the spontaneous activity of large-scale networks, often constrained by structural connectivity from diffusion MRI. While these models capture key resting-state features, including functional connectivity dynamics, their application to cognitive processes remains limited. Cognitive states involve transient, task-specific activations, recruiting distinct brain networks depending on the task demands. A crucial step forward is the incorporation of task-driven constraints into whole-brain models to explore how neuronal populations coordinate during cognitive processes.

#### Cognitive Models: The Role of ACT-R

One of the most influential frameworks in cognitive modeling is the **Adaptive Control of Thought—Rational (ACT-R)** architecture. ACT-R is a computational cognitive architecture designed to simulate human thought processes. It is based on a modular structure where different components correspond to distinct cognitive functions, such as memory retrieval, perceptual processing, and motor execution. These modules communicate through a central procedural system, which selects rules for action based on environmental stimuli and internal goals.

ACT-R has been used extensively in psychology and artificial intelligence to model problem-solving, learning, and decision-making processes. Its symbolic and subsymbolic mechanisms allow it to represent both high-level cognitive functions (e.g., language processing) and more fine-grained adaptations based on experience. While ACT-R provides a robust framework for simulating cognition, its connection to the neurobiological substrate remains an open challenge.

#### Towards a Unified Framework: Linking Brain Activity Models with Cognitive Models

To advance cognitive neuroscience, we need to bridge the gap between models of brain dynamics and cognitive architectures like ACT-R. A promising approach is to constrain whole-brain simulations with task-based empirical data, ensuring that the simulated neural activity reflects cognitive task execution. Several strategies could facilitate this integration:

- Task-Evoked Connectivity: Incorporating experimental data from task-based fMRI or MEG studies to modulate network interactions dynamically.
- Neurophysiological Constraints: Embedding neurophysiological principles (e.g., neural adaptation, synaptic plasticity) into cognitive models to generate biologically plausible outputs.
- Hybrid Models: Combining symbolic cognitive architectures (like ACT-R) with neural mass models or spiking network models to simulate cognitive processes at multiple levels of abstraction.
- Predictive Validation: Using cognitive models to generate testable predictions about brain activity, which can be compared against empirical neuroimaging or electrophysiological data.

#### Future Directions and Applications

Integrating whole-brain modeling with cognitive modeling has profound implications for understanding cognition and its disorders. This approach could help decode how large-scale brain networks adapt to different cognitive demands, shedding light on individual differences in problem-solving and decision-making. Moreover, it offers a potential framework for studying cognitive dysfunction in neurological and psychiatric conditions, where deviations from normative brain dynamics impact cognitive performance.

By leveraging insights from both neuroscience and cognitive science, we can move toward a more comprehensive understanding of how the brain supports intelligent behavior, ultimately refining our ability to model and predict cognitive processes in real-world scenarios.



----





## Art Projects



### Project - Music

> subtitle: ¿?



blabla ... 



### Project - Poetry

> subtitle: ¿?



blabla ... 