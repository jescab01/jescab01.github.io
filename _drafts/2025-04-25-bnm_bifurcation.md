---
layout: post

title: Bifurcations in a brain network model
description: and its relationship with the bifurcations of single nodes (JR NMMs) composing the network
thumbnail: assets/img/bnm-bif_inTime.png
date: 2025/04/25 10:16:04
# in terminal: Get-Date -Format "yyyy/MM/dd HH:mm:ss" ;

tags: jr bnm
categories: models

related_projects: [ "Brain activity" ]

giscus_comments: true

featured: false
---


The brain is a complex system of interacting regions, and understanding its function requires more than studying its
isolated parts. Brain network models (BNM) offer a powerful framework to simulate and analyze large-scale brain dynamics by
combining structural connectivity with models of neural activity (neural mass models as the Jansen-Rit).
These models help us explore how local processes and
global architecture give rise to patterns like oscillations, synchronization, and resting-state networks. In this post,
I share an outlook on BNM bifurcations comparing them with the bifurcation of its composing single nodes. In the following
figure, a BNM parameterized with standard parameters, HCPex atlas downsampled to 52 regions, noise==0.001, and *g*==70 (after a 
first fitting round). Note the name of the regions, along with their average SC weights.

<!-- Row with 1 figure -->
<div class="row mt-4">
  <div class="col-md-12 mb-4">
    <iframe width="100%" height="1000px" src="/assets/html/1-regional-p-plus.html"
      frameborder="0" scrolling="no" allowfullscreen></iframe>
  </div>
</div>


Very interestingly, we can differentiate in that figure the BNM's bifurcations from the NMM's one ("ref" trace). 
What's most striking is that they seem to be independent. Both bifurcations are related to input: interregional
afferences in the BNM, mean intrinsic input in the single node. I would have thought that both inputs are complementary
so, higher SC weight would mean higher input for the region, and this would close the bifurcation for the node 
as in the case of modulating *p*. That's NOT the case. BNM bifurcation closes much earlier and, when it closes, 
it respects the underlying limit cycle of the single node that depends on *p*. It's not able to close further. 
**Somehow, both bifurcations are independent**. And now, question: when we say that we set the BNM at bifurcation, are we
refering to the proper BNM bifurcation, to the single node bifurcation, or both? Should both levels of the system be operating at
criticality? And most importantly, if set at bifurcation, are there actual changes in the behaviour of the system due
to noisy fluctuations? *Let's explore those bifurcations in time in the next figure*.

<!-- Row with 1 figure -->
<div class="row mt-4">
  <div class="col-md-12 mb-4">
    <iframe width="100%" height="400px" src="/assets/html/regional-p-overTime_vRep.html"
      frameborder="0" scrolling="no" allowfullscreen></iframe>
  </div>
</div>

The figure indicates that at least for the level of noise used in this simulation, 
there are no changes in the dynamics, the tendency is to stability.
This is a fascinating starting point -to me-, it would be able to capture fluctuations in the behaviour of the system
in time. Under which circumstances do they actually happen?


> Hey! You can play around with the colors (clicking on the color variable box) of the plots:
> **rFC** (emp-sim PLV correlation), power and *p* - in the case of the 3D scatters - are my favourites. 
> Also, feel free to remove the "ref" trace (clicking on the legend) when it becomes unnecessarily persistent, 
> and decide on what rep (simulation repetition; click them out) you like the most.