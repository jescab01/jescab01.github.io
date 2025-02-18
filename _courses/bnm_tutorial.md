---
layout: page
title: Brain Network Models
description: an introductory tutorial on how to simulate a whole brain activity from empirical data using TVB.
img: assets/img/5.jpg
importance: 1
category: BrainSimulation
---

{::nomarkdown}
{% assign jupyter_path = 'assets/jupyter/tutorial_BrainSimulation-master/Tutorial_BrainNetworkModels.ipynb' | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/tutorial_BrainSimulation-master/Tutorial_BrainNetworkModels.ipynb %}{% endcapture %}
{% if notebook_exists == 'true' %}
  {% jupyter_notebook jupyter_path %}
{% else %}
  <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
