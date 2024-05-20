---
layout: paper
categories: papers
permalink: papers/anomalyclip
id: anomalyclip
title: "Delving into CLIP latent space for Video Anomaly Recognition"
authors: 
  - Luca Zanella*
  - Benedetta Liberatori*
  - Willi Menapace
  - Fabio Poiesi
  - Yiming Wang
  - Elisa Ricci
venue: preprint
venue-shorthand: 
location: 
year: 2023
url: /papers/anomalyclip
pdf: https://arxiv.org/abs/2404.03085
type: preprint
figure: /images/papers/cviu-2023-teaser.png
doi: 
selected: true
feature-title: Delving into CLIP latent space for Video Anomaly Recognition
feature-description: 
image: /images/featured/cviu-2023-method.png
featured: true
feature-order: 1
coming-soon: false
bibtex: |-

    @article{zanella2023delving,
    title={Delving into CLIP latent space for Video Anomaly Recognition},
    author={Zanella, Luca and Liberatori, Benedetta and Menapace, Willi and Poiesi, Fabio and Wang, Yiming and Ricci, Elisa},
    journal={arXiv},
    year={2023}
    }
---

We tackle the complex problem of detecting and recognising anomalies in surveillance videos at the
frame level, utilising only video-level supervision. We introduce the novel method AnomalyCLIP,
the first to combine Large Language and Vision (LLV) models, such as CLIP, with multiple instance
learning for joint video anomaly detection and classification. Our approach specifically involves manipulating the latent CLIP feature space to identify the normal event subspace, which in turn allows
us to effectively learn text-driven directions for abnormal events. When anomalous frames are projected onto these directions, they exhibit a large feature magnitude if they belong to a particular class.
We also introduce a computationally efficient Transformer architecture to model short- and long-term
temporal dependencies between frames, ultimately producing the final anomaly score and class prediction probabilities. We compare AnomalyCLIP against state-of-the-art methods considering three
major anomaly detection benchmarks, i.e. ShanghaiTech, UCF-Crime, and XD-Violence, and empirically show that it outperforms baselines in recognising video anomalies.
