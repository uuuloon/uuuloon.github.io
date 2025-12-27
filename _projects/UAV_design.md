---
layout: page
title: UAV Design
description: Drone design for TDK 25th Robotics Competition, UAV group
img: assets/img/UAV.jpg
redirect:
importance: 2
category: undergrad
---

The team consist of 6 members, and this competition aim to compete for the aerial robot's capability in autonomous flight, object detection, precision, and stability. I was mainly responsible for the machanical design for the drone, and I also reconstructed the a trapezoidal cube obstacle (Salt Mountain) in the competition for algorithm evaluation. Below is the demo for the line following function and Salt Mountain.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0" style="flex: 1.79;">
        {% include figure.liquid path="assets/img/LineFollowing.gif" caption="Line following demo" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0" style="flex: 0.55;">
        {% include figure.liquid path="assets/img/SaltMountain.gif" caption="Salt Mountain" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Here is the video that I teleoperated the UAV in the trial to collect data for autonomous line tracking.

<figure class="video-wide" style="text-align:center">
  {% include video.liquid path="https://www.youtube.com/embed/8fdv2UCUNq8" width="100%" %}
  <figcaption><em>Teleoperation in trial for TDK Competition</em></figcaption>
</figure>

Competition report and technical documentation translated from Traditional Chinese is available below.

<div class="row justify-content-sm-center">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include pdf.liquid path="assets/pdf/TDK_report.pdf" caption="Technical report" %}
    </div>
</div>
