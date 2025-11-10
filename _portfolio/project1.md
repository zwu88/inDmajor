---
title: Symphony Orchestra of the Student Strings Association
subtitle: TANTE (Time-Adaptive Transformer with Neural Taylor Expansion) is a new operator-learning framework for time-dependent PDEs that uses neural Taylor expansion to make accurate, continuous-time predictions with adaptive step sizes, improving both accuracy and efficiency over fixed-step methods.
image: assets/img/paper/tante_video.gif
alt: tante video

caption:
  title: TANTE (May 19, 2025)
  subtitle: Time-Adaptive Operator Learning via Neural Taylor Expansion. (Operator Learning, Scientific Machine Learning, PDEs)
  thumbnail: assets/img/paper/tante_video_vertical.gif
---



## 🔎 Abstract

<style>
  .about { text-align: left; } 
  @media (min-width: 768px) {
    .about { text-align: justify; }
  }
</style>

<p class="about">
Operator learning for time-dependent partial differential equations (PDEs) has seen rapid progress in recent years, enabling efficient approximation of complex spatiotemporal dynamics. However, most existing methods rely on fixed time step sizes during rollout, which limits their ability to adapt to varying temporal complexity and often leads to error accumulation. To address this gap, we propose the Time-Adaptive Transformer with Neural Taylor Expansion (TANTE), a novel operator-learning framework that produces continuous-time predictions with adaptive step sizes. TANTE predicts future states by performing a Taylor expansion at the current state, where neural networks learn both the higher-order temporal derivatives and the local radius of convergence. This allows the model to dynamically adjust its rollout based on the local behavior of the solution, thereby reducing cumulative error and improving computational efficiency. We demonstrate the effectiveness of TANTE across a wide range of PDE benchmarks, achieving superior accuracy and adaptability compared to fixed-step baselines, delivering accuracy gains of 10-50% and speed-ups of 30-80% at inference.
</p>

## 🧱 Pipeline

<p align="center"> <img src="assets/img/paper/tante_pipeline.jpg" width="88%"> </p>

<p class="about">
Time-Adaptive Transformer with Neural Taylor Expansion (TANTE). Our framework enables continuous-time prediction with dynamically adjusted step sizes based on local temporal complexity. TANTE generates forecasts by summing the predicted derivatives as a Taylor series within the confidence interval.
</p>

## 🏆 Main Results

<p align="center"> <img src="assets/img/paper/tante_table.jpg" width="90%"> </p>

{: .text-justify } 
> L2RE (↓ lower is better) of rollouts on *T'* time points on four benchmarks (*TR*, *AM*, *VF*, and *RB*). Results are divided into three parts based on different model sizes. In each part, the best results are **bolded** and the second-best results are **underlined**. We **highlight** the globally best results using **blue** and mark our TANTE models with **red font**.

---

{:.text-left}
- Date: May 19, 2025
- Paper: [TANTE: Time-Adaptive Operator Learning via Neural Taylor Expansion](http://arxiv.org/abs/2502.08574)
- Code: [Github Repo of TANTE](https://github.com/zwu88/TANTE)
- Authors: **Zhikai Wu**, Sifan Wang, Shiyang Zhang, Sizhuang He, Min Zhu, Anran Jiao, Lu Lu, David van Dijk
- Laboratory: [van Dijk Lab @Yale](https://www.vandijklab.org)
- Previous Project: [COAST: Intelligent Time-Adaptive Neural Operators](https://arxiv.org/abs/2502.08574v1) (legacy)
