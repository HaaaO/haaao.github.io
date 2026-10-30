---
layout: paper
categories: papers
permalink: papers/pedbench-2026
id: pedbench-2026
title: "PEDBench: Can Speech Models Detect Phonetic Errors?"
authors:
  - Zhonghao Shi
  - Zackary Rackauckas
  - Jasmine Yip
  - Savannah Halpern
  - Simon Campos
  - Lauren Brace
  - Emma Yang
  - Tiantian Feng
  - Xuan Shi
  - Shrikanth Narayanan
  - Teresa Satterfield
  - Ying Xu
venue: arXiv preprint
venue-shorthand: arXiv
year: 2026
url: /papers/pedbench-2026
pdf: https://arxiv.org/pdf/2610.20830
type: preprint
feature-title: PEDBench
feature-description: "We introduced PEDBench, the first phonetic error detection benchmark spanning real children's speech, acted errors, and synthetic errors, and showed that 13 state-of-the-art speech models fail to reliably detect phonetic errors."
featured: false
bibtex: |-

  @article{shi2026pedbench,
  title={PEDBench: Can Speech Models Detect Phonetic Errors?},
  author={Shi, Zhonghao and Rackauckas, Zackary and Yip, Jasmine and Halpern, Savannah and Campos, Simon and Brace, Lauren and Yang, Emma and Feng, Tiantian and Shi, Xuan and Narayanan, Shrikanth and Satterfield, Teresa and Xu, Ying},
  journal={arXiv preprint arXiv:2610.20830},
  year={2026}
  }
---

Phonetic error detection (PED) aims to identify phoneme-level substitutions, deletions, and insertions and is essential for educational and clinical speech assessment and intervention. Despite recent advances in speech models for phoneme recognition, their ability to reliably detect fine-grained phonetic errors remains unclear because of a lack of high-quality evaluation data. To address this gap, we introduce PEDBench, the first PED benchmark spanning a continuum from natural to controlled speech. It comprises real-world recordings of spoken errors made by children (N=334), scripted error productions by human actors (N=1,188), and synthetic error productions generated using phone-conditioned text-to-speech (N=1,083). All phonetic annotations were transcribed and verified by two phonetically trained annotators. Our evaluation of 13 state-of-the-art speech models shows that they fail to reliably detect phonetic errors, even under controlled conditions with acted and synthetic speech, where acoustic variability is reduced. The models also exhibit low precision, frequently misclassifying correctly pronounced phonemes as errors. Our speech-language models, fine-tuned on synthetic data, outperform commercial and open-source baselines on word-level PED, although a sim-to-real domain gap remains. We plan to publicly release our code and recipes, along with our acted and synthetic datasets, to support the development of more accurate PED systems.
