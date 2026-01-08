---
layout: default
img: assets/img/publication_preview/feasibility.jpg
importance: 1
category: research
---

<div class="container text-center">
  <h1 style="color: #48BB78; font-weight: bold; font-family: 'Times New Roman', serif;">Feasibility-Guided Planning over Multi-Specialized<br>Locomotion Policies</h1>
  
  <p class="mt-3" style="font-size: 1.2rem;">ICRA 2026 (under review)</p>
  
  <p class="mt-3" style="font-size: 1.1rem; font-style: italic;">
    <a href="https://ysluo.github.io/">Ying-Sheng Luo</a>, <a href="https://richard98hess444.github.io/">Lu-Ching Wang</a>, <a href="https://scholar.google.com/citations?user=984Gl4gAAAAJ&hl=en">Hanjaya Mandala</a>, <span style="font-weight: bold;">Yu-Lun Chou</span>, <a href="https://guichristmann.com/">Guilherme Henrique Galelli Christmann</a>, <a href="https://github.com/YuZhong-Chen">Yu-Chung Chen</a>, <a href="https://github.com/Assume-Zhan">Yung-Shun Chan</a>, <a href="https://scholar.google.com/citations?user=5mYNdo0AAAAJ&hl=zh-TW">Chun-Yi Lee</a>, <a href="https://scholar.google.com/citations?user=bndb0gYAAAAJ&hl=en">Wei-Chao Chen</a>
  </p>

  <figure class="video-wide" style="text-align:center">
    {% include video.liquid path="https://www.youtube.com/embed/rkdNR5ZwDTQ" width="100%" %}
  </figure>
</div>

<div class="container mt-5">
  <h2 style="color: #48BB78; font-weight: bold;">Abstract</h2>
  
  <p class="mt-4" style="text-align: justify; line-height: 1.6;">
    Planning over unstructured terrain presents a significant challenge in the field of legged robotics. Although recent works in reinforcement learning have yielded various locomotion strategies, planning over multiple experts remains a complex issue. Existing approaches encounter several constraints: traditional planners are unable to integrate skill-specific policies, whereas hierarchical learning frameworks often lose interpretability and require retraining whenever new policies are added. In this paper, we propose a feasibility-guided planning framework that successfully incorporates multiple terrain-specific policies. Each policy is paired with a Feasibility-Net, which learned to predict feasibility tensors based on the local elevation maps and task vectors. This integration allows classical planning algorithms to derive optimal paths. Through both simulated and real-world experiments, we demonstrate that our method efficiently generates reliable plans across diverse and challenging terrains, while consistently aligning with the capabilities of the underlying policies.
  </p>
</div>
