---
layout: paper
categories: papers
permalink: papers/convisbench
id: convisbench
title: "ConViS-Bench: Estimating Video Similarity Through Semantic Concepts"
authors: 
  - Benedetta Liberatori
  - Lorenzo Vaquero
  - Alessandro Conti 
  - Yiming Wang
  - Elisa Ricci
  - Paolo Rota
  
venue: Annual Conference on Neural Information Processing Systems
venue-shorthand: NeurIPS
location: San Diego, California, USA
year: 2025
url: https://benedettaliberatori.github.io/convisbench/
pdf: https://arxiv.org/pdf/2509.19245
project: https://benedettaliberatori.github.io/convisbench/
poster: https://neurips.cc/media/PosterPDFs/NeurIPS%202025/121680.png?t=1764512133.0262516
doi: 
type: conference
figure: /images/papers/neurips-2025-dataflow.png
selected: true
feature-title: "ConViS-Bench: Estimating Video Similarity Through Semantic Concepts"
feature-description: 
image: /images/papers/neurips-2025-dataflow.png
featured: true
feature-order: 0
coming-soon: false
bibtex: |-

  @inproceedings{liberatori2025convisbench,
  title={ConViS-Bench: Estimating Video Similarity  Through Semantic Concepts},
  author={Benedetta Liberatori and Alessandro Conti and Lorenzo Vaquero and Yiming Wang and Elisa Ricci and Paolo Rota},
  booktitle={The Thirty-ninth Annual Conference on Neural Information Processing Systems Datasets and Benchmarks Track},
  year={2025},
  url={https://openreview.net/forum?id=NoIWLerNKH}
  }
---

What does it mean for two videos to be similar? Videos may appear similar when judged by the actions they depict, yet entirely different if evaluated based on the locations where they were filmed. While humans naturally compare videos by taking different aspects into account, this ability has not been thoroughly studied and presents a challenge for models that often depend on broad global similarity scores. Large Multimodal Models (LMMs) with video understanding capabilities open new opportunities for leveraging natural language in comparative video tasks. We introduce Concept-based Video Similarity estimation (ConViS), a novel task that compares pairs of videos by computing interpretable similarity scores across a predefined set of key semantic concepts. ConViS allows for human-like reasoning about video similarity and enables new applications such as concept-conditioned video retrieval. To support this task, we also introduce ConViS-Bench, a new benchmark comprising carefully annotated video pairs spanning multiple domains. Each pair comes with concept-level similarity scores and textual descriptions of both differences and similarities. Additionally, we benchmark several state-of-the-art models on ConViS, providing insights into their alignment with human judgments. Our results reveal significant performance differences on ConViS, indicating that some concepts present greater challenges for estimating video similarity. We believe that ConViS-Bench will serve as a valuable resource for advancing research in language-driven video understanding.