---
layout: page
title: Vision-Language Navigation (VLN)
description: Visual-Language Action model Research for robotic navigation in unseen environments.
img: assets/img/VLN.gif
redirect:
importance: 1
category: work
---

<div class="container mt-5">
  <h3 style="color: #48BB78; font-weight: bold;">Introduction</h3>
  
  <p class="mt-4" style="text-align: justify; line-height: 1.6;">
    Built on <a href="https://navila-bot.github.io/">NaVILA</a> (Cheng et al), a universal Vision-Language-Action (VLA) model that lets legged robots navigate via natural-language instructions, this project deploys and evaluates VLN on a Unitree A1 quadruped. Below are indoor deployment demonstrations; see <a href="https://inventec-ai-center.github.io/vl-n3rd-bench/">VL-N3RD-Bench</a> for our benchmark of 3D reconstruction pipelines for sim-to-real deployment.

  </p>
</div>

<figure class="video-wide" style="text-align:center">
  {% include video.liquid path="https://www.youtube.com/embed/Lhw8eWcdAa8" width="100%" %}
  <figcaption><em>Simple VLN tasks following natural-language navigation instructions</em></figcaption>
</figure>

<figure class="video-wide" style="text-align:center">
  {% include video.liquid path="https://www.youtube.com/embed/uL2eC20qQmw" width="100%" %}
  <figcaption><em>Long-Horizon VLN task</em></figcaption>
</figure>

<div class="container mt-5">
  <h3 style="color: #48BB78; font-weight: bold;">System Requirements</h3>
  
  <p class="mt-4" style="text-align: justify; line-height: 1.6;">
    We install the conda environment for NaVILA and run the VLN model on the server with RTX 5090 GPU. Since the paper used 40-series for the setup, there's some incompatibility with the 50-series. For a detailed setup guide, please refer to <a href="https://richard98hess444.github.io/other/NaVILA_Installation.md">this</a> instruction written by <a href="https://richard98hess444.github.io/">Richard Wang</a>. 
  </p>
</div>
