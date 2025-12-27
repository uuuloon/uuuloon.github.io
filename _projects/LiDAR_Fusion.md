---
layout: page
title: Dual-LiDAR Fusion SLAM
description: Fuse point cloud data from dual LiDARs to accelerate SLAM performance in QRC 2025.
img: assets/img/mapping_demo.gif
importance: 4
category: work
---

The system configuration is shown in the left image. The dual-LiDAR setup provides 315° coverage and reduces 65 % mapping time comparing to single LiDAR, enabling fast, single-pass mapping in dynamic environments of [QRC 2025](https://2025.ieee-icra.org/competitions/#qrc). The real-time fused point cloud is shown on the right.

<div class="row d-flex align-items-start">
    <div class="col-sm mt-3 mt-md-0" style="flex: 0.75;">
        {% include figure.liquid path="assets/img/TwoLivox.jpeg" caption="Dual LiDAR Scanner" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0" style="flex: 1.06;">
        {% include figure.liquid path="assets/img/Dual_LiDAR_SLAM.gif" caption="Real-time point cloud fusion" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

During the competition, I was responsible for mapping various terrains, including all six shown here.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/QRC_terrains.png" caption="QRC terrains" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Take the sand and gravel as an example, the terrain and scanned map are shown below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/sand_gravel.png" caption="Sand and gravel terrain" class="img-fluid rounded z-depth-1 img-equal-height" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/sand_gravel_scan.png" caption="Point cloud scan" class="img-fluid rounded z-depth-1 img-equal-height" %}
    </div>
</div>

Since the raw scanning data is usually noisy, filtering is required to remove outliers. Then, the filtered map is converted into a height map, allowing the robot to plan and navigate using feasible trajectories.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/sand_gravel_heightmap.png" caption="Height map" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Here's other mapping results for consecutive terrains.

<div class="row d-flex align-items-start">
    <div class="col-sm mt-3 mt-md-0" style="flex: 1.66;">
        {% include figure.liquid path="assets/img/QRC_Lane1.png" caption="Lane1" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0" style="flex: 3.23;">
        {% include figure.liquid path="assets/img/Lane1_heightmap.png" caption="Lane1 height map (rotating ramps, soft foam, pallets and pipes)" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="row d-flex align-items-start">
    <div class="col-sm mt-3 mt-md-0" style="flex: 1.64;">
        {% include figure.liquid path="assets/img/QRC_Lane2.png" caption="Lane2" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0" style="flex: 3.32;">
        {% include figure.liquid path="assets/img/Lane2_heightmap.png" caption="Lane2 height map (sand and gravel, k-rails, stairs)" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

---

## Limitations and Future Work

Although the robot can plan feasible trajectories, localization instablility causes drift and navigation failure. This is mainly due to the limited ceiling features and dynamic environment in the stadium, which challenge conventional LiDAR-based localization. Under these conditions, upward-facing LiDAR is ineffective, motivating future exploration of alternative sensing configurations or localization methods.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Limited_ceiling_features.gif" caption="Limited ceiling features" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
