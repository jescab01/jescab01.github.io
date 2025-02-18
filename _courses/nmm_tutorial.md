---
layout: page
title: Neural Mass Models
description: an introductory tutorial to some of the equations available to reproduce brain activity.
img: assets/img/3.jpg
importance: 2
category: BrainSimulation
---

{::nomarkdown}
{% assign jupyter_path = 'assets/jupyter/tutorial_BrainSimulation-master/Tutorial_NeuralMasses.ipynb' | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/tutorial_BrainSimulation-master/Tutorial_NeuralMasses.ipynb %}{% endcapture %}
{% if notebook_exists == 'true' %}
  {% jupyter_notebook jupyter_path %}
{% else %}
  <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
