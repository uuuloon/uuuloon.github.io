---
layout: page
title: Dual-LiDAR Fusion SLAM
description: Fuse point cloud data from dual LiDARs to accelerate SLAM performance in QRC 2025 (click for pipeline details).
img: assets/img/mapping_demo.gif
importance: 4
category: work
---

The system configuration is shown below. The dual-LiDAR setup provides 270° coverage, enabling fast, single-pass mapping in dynamic environments.

<img src="/assets/img/TwoLivox.jpeg" width="225" height="300">

During QRC 2025, I was responsible for mapping various competition terrains (e.g., sand and gravel).

<img src="/assets/img/sand_gravel.png" width="300" height="200">
<img src="/assets/img/sand_gravel_scan.png" width="300" height="210">

Then, the point cloud map is converted into a height map, allowing the robot to plan and navigate using feasible trajectories.

<img src="/assets/img/sand_gravel_heightmap.png" width="300" height="190">
