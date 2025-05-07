---
layout: post

title: Bifurcations in a brain network model
description: and its relationship with the bifurcations of single nodes (JR NMMs) composing the network
thumbnail: assets/img/bnm-bifs-jr.png
date: 2025/05/07 12:41:17
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
figure, a BNM parameterized with standard JR parameters, noise==0.001, and SC based on DK atlas. First, I show
in 2D the effect of g on the bifurcation, including all left hemisphere regions simulated. Regions were sorted
in ascending order for increasing SC weights. Note the name of the regions, along with their average SC weights.

<!-- Row with 1 figure -->
<div class="row mt-4">
  <div class="col-md-12 mb-4">
    <iframe width="100%" height="1300px" src="/assets/html/1regional-bifs.html"
      frameborder="0" scrolling="no" allowfullscreen></iframe>
  </div>
</div>


In that figure, we can compare the BNM's bifurcations as g is increasing with the bifurcation of the single NMM ("ref" trace). 
Both bifurcations are related to input: interregional
afferences in the BNM, mean intrinsic input in the single node. Therefore, they have a complementary effect over the
bifurcation: higher SC weight would mean higher input for the region, and thus a further position in the bifurcation
with respect to the single node bifurcation. The higher the SC weights the earlier the bifurcation closes.

Finally, check out this other perspective on the same data. 3D scatters for bifurcations in g and p, 
with additional variables to color the datapoints. 

<!-- Row with 1 figure -->
<div class="row mt-4">
  <div class="col-md-12 mb-4">
    <iframe width="100%" height="400px" src="/assets/html/2regional_sub-p-g.html"
      frameborder="0" scrolling="no" allowfullscreen></iframe>
  </div>
</div>

> Hey! You can play around with the colors (clicking on the color variable box) of the plots:
> **rFC** (emp-sim PLV correlation), power and *g* are my favourites. 
> Also, feel free to remove the "ref" trace (clicking on the legend) when it becomes unnecessarily persistent.