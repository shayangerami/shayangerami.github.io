---
layout: page
title: ROAST
description: Bit-flip attack on the learned sampling offsets of LBPNet (DAC 2026, Late Breaking Results)
img: # optional card image, e.g. assets/img/projects/roast.jpg
importance: 6
category: research
related_publications: true
---

**ROAST: Reverse-training Offset Attack on Spatial Sampling Topologies** {% cite gerami2026roast %}

Lightweight vision networks such as LBPNet learn where to sample pixels. ROAST evaluates how robust those learned spatial sampling offsets are to hardware bit-flip faults.

#### Highlights

- Developed a white-box attack on LBPNet that maximizes classification loss by updating the learned spatial sampling offsets, then uses truncated Hamming distance on their FP32 representations to construct a bit-flip schedule.
- Evaluated independent and cumulative attacks on MNIST and SVHN, reducing accuracy by 69.52 and 64.42 percentage points while flipping only 4.39% and 4.52% of offset bits, respectively.
- Achieved greater accuracy degradation per flipped bit than the Bit-Flip Attack (BFA).
