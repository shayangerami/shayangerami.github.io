---
layout: page
title: Heatmap-Guided LBPNet
description: Heatmap-guided adaptive LBP for efficient in-sensor visual recognition (IEEE JETCAS)
img: # optional card image, e.g. assets/img/projects/heatmap-lbpnet.jpg
importance: 4
category: research
github: https://github.com/shayangerami/HeatMapLBPNET
related_publications: true
---

**Pixel-Wise Intelligence: Heatmap-Guided Adaptive LBP for In-Sensor Vision Processing** {% cite gerami2026pixelwise %}

LBPNet replaces multiply-accumulate operations with local binary pattern comparisons, which suits in-sensor processing. This work focuses LBPNet's computation on informative image regions instead of spending it on the background.

#### Highlights

- Introduced heatmap-guided spatial masking and adaptive sampling for the MAC-free LBPNet architecture.
- Reduced operations by more than 10× and model size by more than 100× compared with CNN baselines on structured vision tasks.
- Achieved approximately 99% accuracy on digit and character recognition and 95% on facial-expression recognition.

Code: [github.com/shayangerami/HeatMapLBPNET](https://github.com/shayangerami/HeatMapLBPNET)
