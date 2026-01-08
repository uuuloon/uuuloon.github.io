---
layout: page
title: Vision-Language Navigation (VLN)
description: Researching VLN for robotic navigation in unseen environments.
img: assets/img/VLN.gif
redirect:
importance: 1
category: work
---

This research is currently in progress. I am exploring how quadruped robots can follow natural-language instructions to navigate novel environments using vision-language models.

<div class="container mt-5">
  <h3 style="color: #48BB78; font-weight: bold;">Introduction</h3>
  
  <p class="mt-4" style="text-align: justify; line-height: 1.6;">
    The framework is built on top of <a href="https://navila-bot.github.io/">NaVILA</a>, which was proposed by Cheng et al. NaVILA is a universal Vision-Language-Action (VLA) model for legged robots to perform navigation through natural-language instructions. For more details, please refer to the their website embeded above.

    Below are recent deployments demonstrating vision-language navigation on a Unitree A1 quadruped in indoor environments.

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

More updates are coming soon. Stay tuned!
