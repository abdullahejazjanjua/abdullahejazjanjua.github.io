---
layout: page
title: Project Showcase
permalink: /project-showcase/
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
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(min(100%, 240px), 1fr));
    gap: 1rem;
    padding: 0;
    list-style: none;
  }

  .project-showcase > li {
    min-width: 0;
  }

  .project-showcase .showcase-card {
    display: block;
    height: 100%;
    padding: 1.25rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.5rem;
    background: var(--global-card-bg-color);
    color: var(--global-text-color);
    text-decoration: none;
    overflow-wrap: anywhere;
    transition: border-color 150ms ease;
  }

  .project-showcase .showcase-card:hover,
  .project-showcase .showcase-card:focus-visible {
    border-color: var(--global-theme-color);
    text-decoration: none;
  }

  .project-showcase .showcase-card:focus-visible {
    outline: 2px solid var(--global-theme-color);
    outline-offset: 3px;
  }

  .project-showcase .showcase-title {
    margin: 0 0 0.5rem;
    color: var(--global-text-color);
    font-size: 1.2rem;
    font-weight: 700;
    line-height: 1.3;
  }

  .project-showcase .showcase-card:hover .showcase-title,
  .project-showcase .showcase-card:focus-visible .showcase-title {
    color: var(--global-theme-color);
  }

  .project-showcase .showcase-description {
    margin: 0;
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    line-height: 1.5;
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
        <h2 class="showcase-title">{{ project.title | escape }}</h2>
        <p class="showcase-description">{{ project.description | escape }}</p>
      </a>
    </li>
  {% endfor %}
</ul>
