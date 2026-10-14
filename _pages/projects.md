---
layout: page
title: projects
permalink: /projects/
description: A selection of my coding projects and experiments.
nav: true
nav_order: 3

# Add projects here using title, description, and url. Cards appear in this order.
projects:
  - title: TinyTorch
    description: A CUDA-native deep learning framework built in C++ with custom GPU kernels, automatic differentiation, and Python bindings.
    url: https://github.com/abdullahejazjanjua/tinytorch
  - title: DINO ResNet50
    description: A PyTorch implementation of self-supervised ResNet training using DINO's student-teacher architecture and knowledge distillation.
    url: https://github.com/abdullahejazjanjua/dinov1-resnet
  - title: Vision Transformer
    description: >-
      A Vision Transformer implemented from scratch in PyTorch, featuring patch embeddings, multi-head attention, and a parallelized attention implementation.
    url: https://github.com/abdullahejazjanjua/vision_transformer
  - title: Variational Autoencoder
    description: A PyTorch variational autoencoder with a ResNet-based encoder and convolutional decoder for generating faces from the CelebA dataset.
    url: https://github.com/abdullahejazjanjua/variational-autoencoder
  - title: RealNVP
    description: A normalizing-flow generative model implemented in PyTorch using invertible affine coupling layers for image density modeling and generation.
    url: https://github.com/abdullahejazjanjua/real-nvp

_styles: |
  .project-showcase {
    margin: 0;
    padding: 0;
    list-style: none;
    border-top: 1px solid var(--global-rule-color);
  }

  .project-showcase > li {
    min-width: 0;
    border-bottom: 1px solid var(--global-rule-color);
  }

  .project-showcase .showcase-card {
    display: block;
    padding: 1.25rem 0;
    color: var(--global-text-color);
    text-decoration: none;
    overflow-wrap: anywhere;
  }

  .project-showcase .showcase-card:hover,
  .project-showcase .showcase-card:focus-visible {
    text-decoration: none;
  }

  .project-showcase .showcase-card:focus-visible {
    outline: 2px solid var(--global-theme-color);
    outline-offset: 3px;
  }

  .project-showcase .showcase-title {
    margin: 0;
    color: var(--global-theme-color);
    text-decoration: underline;
    text-underline-offset: 0.2em;
    text-decoration-thickness: 1px;
    font-size: 1.125rem;
    font-weight: 500;
    line-height: 1.4;
  }

  .project-showcase .showcase-card:hover .showcase-title,
  .project-showcase .showcase-card:focus-visible .showcase-title {
    color: var(--global-hover-color);
  }

  .project-showcase .showcase-description {
    margin: 0.5rem 0 0;
    max-width: 46rem;
    color: var(--global-text-color-light);
    font-size: 0.9375rem;
    line-height: 1.65;
  }

  .project-showcase .showcase-heading {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    gap: 1rem;
  }

  .project-showcase .showcase-destination {
    flex-shrink: 0;
    color: var(--global-theme-color);
    font-size: 0.8125rem;
    text-decoration: underline;
    text-underline-offset: 0.2em;
  }

  .project-showcase .showcase-card:hover .showcase-destination {
    color: var(--global-hover-color);
  }

  @media (max-width: 400px) {
    .project-showcase .showcase-heading {
      flex-wrap: wrap;
      gap: 0.25rem 1rem;
    }
  }
---

{% comment %}
To add a card, copy an entry in the projects list above and edit its three fields.
Use a full URL for external links or a root-relative path for pages on this site.
{% endcomment %}

<ul class="project-showcase">
  {% for project in page.projects %}
    <li>
      <a class="showcase-card" href="{{ project.url | relative_url | escape }}">
        <div class="showcase-heading">
          <h2 class="showcase-title">{{ project.title | escape }}</h2>
          <span class="showcase-destination">view project <span aria-hidden="true">↗</span></span>
        </div>
        <p class="showcase-description">{{ project.description | escape }}</p>
      </a>
    </li>
  {% endfor %}
</ul>
