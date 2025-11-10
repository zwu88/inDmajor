---
title: "Conductor, Yuanpei Acoustic Chamber Choir"
subtitle: Serving as conductor since Mar 2024.
image: assets/img/paper/gcpnet_pipeline.jpg
alt: GCPNet pipeline

caption:
  title: GCPNet (CISP-BMEI 2024)
  subtitle: Predicting Microbial Community Productivity with Graph Neural Networks. (Computational Biology, GNNs)
  thumbnail: assets/img/paper/gcpnet_pipeline_high.jpg
---
## 🔎 Abstract

<style>
  .about { text-align: left; } 
  @media (min-width: 768px) {
    .about { text-align: justify; }
  }
</style>

<p class="about">
Artificial microbial community design has gained increasing attention due to its economic and environmental benefits. However, it is challenging considering the complex microbial interactions and emergent properties arising from metabolic networks. Although flux balance analysis (FBA), based on genome-scale metabolic models (GEMs), is a well-known approach for simulating community phenotypes, its inefficiency in handling communities with a large number of functional genes limits its utility. In this paper, we introduce a novel graph neural network model that incorporates growth-coupling effects to predict the productivity of microbial communities, which is impractical for prior techniques. Utilizing 83 high-quality bacterial GEMs, we trained and tested our model on a large number of bacterial communities containing two or three strains, each undergoing a random genetic modification (either knock-outs or knock-ins) within the community GEM. Our model demonstrates high concordance with FBA, achieving an average area under the curve (AUC) of 0.98, and a F1 score of 0.82. Notably, it operates approximately 6,415 times faster than FBA. Our model indicates that graph-based machine learning algorithms can significantly accelerate productivity prediction and hold potential to advance microbial community design, thereby guiding microbial engineering strategies.
</p>

## 🧱 Pipeline

<p align="center"> <img src="assets/img/paper/gcpnet_pipeline.jpg" width="88%"> </p>

{:.text-left}
1. Genome Annotation → Feature Matrix
2. Metabolic Similarity & Exchange → Graph Construction
3. GNN Encoder → Productivity Regressor

---

{:.text-left}
- Date: Oct 26, 2024
- DOI: [10.1109/CISP-BMEI64163.2024.10906150](https://doi.org/10.1109/CISP-BMEI64163.2024.10906150)
- Venue: *17th International Congress on Image and Signal Processing, Biomedical Engineering & Informatics (CISP-BMEI 2024)*
- Authors: Jiaheng Hou, Peter X. Geng, **Zhikai Wu**, Wenlin Fan, Huaiqiu Zhu
- Laboratory: Zhu Lab @Peking University
