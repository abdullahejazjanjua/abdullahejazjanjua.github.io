---
layout: about
title: about
permalink: /
subtitle: Talent is a pursued interest. Anything that you're willing to practice, you can do.

profile:
  align: right
  image: profile_pic.png
  image_alt: Portrait of Abdullah Ejaz Janjua
  image_circular: false # crops the image to make it circular
  role: Computer Science Undergraduate
  location: GIKI, Pakistan
  location_url: https://giki.edu.pk

selected_papers: False # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

# Copy an entry to add an achievement. year accepts a year or range (e.g. 2023–present).
# Descriptions support Markdown. No HTML or CSS edits are needed.
achievements:
  - title: Mitacs Globalink Research Internship
    year: "2026"
    description: >-
      Selected for the competitive, fully funded Mitacs Globalink Research Internship to conduct research on diffusion models and subject personalization at Carleton University, Canada, under [Dr. Junfeng Wen](#).
  - title: Deans Honor Roll
    year: "2023–present"
    description: >-
      Achieved a CGPA of 3.78/4.00, ranking 4th among 41 students in my class and 13th among 631 students in my batch. Earned consequentive Dean's Honor Roll Distinction in every semester to date.

# Add projects using title, description, and url. They appear below Achievements in this order.
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

announcements:
  enabled: False # includes a list of news items
  scrollable: False # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: False
  scrollable: False # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a final-year Computer Science undergraduate at the Ghulam Ishaq Khan Institute of Engineering Sciences and Technology. While my prior research centers on computer vision and generative modeling, my primary technical interest lies in low-level systems for machine learning: optimizing inference, writing custom GPU kernels, and making neural networks run faster and more efficiently on hardware.

Currently, I am working with [Dr. Junfeng Wen](https://junfengwen.github.io/) at Carleton University on adapting pre-trained diffusion models along the temporal axis to model continuous facial aging. Prior to this, I conducted research at the Intelligent Machines Lab under [Dr. Waqas Sultani](https://waqassultani.github.io/) on domain generalization for DETR architectures and unsupervised domain adaptation for microscopy imaging. Alongside my research, I actively explore systems-level performance, which includes developing [TinyTorch](https://github.com/abdullahejazjanjua/tinytorch), a custom C++/CUDA deep learning framework with handcrafted, fused GPU kernels and an autograd engine from scratch.

When I am away from the keyboard, I read manga, manhwa, and light novels, and spend time playing narrative-driven video games like Red Dead Redemption 2, The Witcher, and Ghost of Tsushima.
