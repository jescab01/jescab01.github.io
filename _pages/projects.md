---
layout: page
title: projects
permalink: /projects/
description: >
  A growing collection of your cool projects.
  
nav: true
nav_order: 2
display_categories: [research] #, art]
horizontal: false
---

  
[//]: # (I spend most of my time dedicated to research projects in computational neuroscience but)
[//]: # (![research-lines]&#40;/assets/img/projects2.png&#41;{: .invert-dark-mode })

My research is centered on developing and applying computational 
models of brain function and its modulation to foster our understanding 
of mental health and disease, cognition and behaviour. While building
and enhancing these computational models is a research endeavour on 
its own, I believe that their true value emerges from
their application to address specific research topics such
as **Alzheimer’s disease** and **wellbeing**.


<div style="display: flex; align-items: center; gap: 20px;">
  <div style="flex: 1;">
    <p>
    The diagram above represents this interconnected framework, 
    where the <b>horizontal axis</b> distinguishes between 
    application domains, while the <b>vertical axis</b> 
    outlines complementary types of models. Each of 
    these approaches contributes independently to neuroscience 
    but gains greater relevance when integrated, enhancing both 
    theoretical insights and practical applications. 
    </p>
    <p>
    Beyond my academic research, I also engage in creative projects, including
    <b>music and poetry</b>, which, in their own way, reflect a complementary 
    exploration of cognition and human expression.
    </p>
  </div>
  <div style="flex: 1;">
    <img src="/assets/img/projects3.png" alt="research-lines" class="invert-dark-mode" style="max-width: 100%; height: auto;">
  </div>
</div>



<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
