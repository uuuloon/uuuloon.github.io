---
layout: page
title: Learning-based Control with Low-level Interface
description: Develop low-level control interface for quadruped robots, with reinforcement learning in IsaacGym and real-world deployment.
img: assets/img/deployment.gif
redirect:
importance: 2
category: work
---

Building from the ground up, I first implemented a low-level control interface using UDP protocol, enabling position control for legs. This interface supports both user-specified target positions and sinusoidal motions. Then, I migrated the interface to [Lightweight Communications and Marshalling](https://lcm-proj.github.io/lcm/), adopting a publisher-subscriber architecture for command input and state feedback.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/PositionControl.gif" caption="User-specified control" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/PositionControl_Sinusoidal.gif" caption="Sinusoidal control" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Built on top of this interface, I deployed an existing gait generator on the real robot, enabling customizable gait patterns (e.g., frequency, amplitude, phase, etc.). Finally, I trained multiple locomotion policies (e.g., flat-ground and general locomotion) in [Isaac Gym](https://developer.nvidia.com/isaac-gym) and deployed them on the real robot. An onboard IMU was also integrated to provide state observations required by the policy.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Gait_Generator.gif" caption="Gait generator" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/IsaacGym_eval.gif" caption="IsaacGym evaluation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Below is the final deployment result demonstrating robust locomotion.

<figure class="video-wide" style="text-align:center">
  {% include video.liquid path="https://www.youtube.com/embed/M_Wu1FNsxcE" width="100%" %}
  <figcaption><em>Walking on a QRC practice terrain</em></figcaption>
</figure>
