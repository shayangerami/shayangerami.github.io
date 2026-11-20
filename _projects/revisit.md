---
layout: page
title: ReVisiT
description: Training-free selective inference for efficient video vision transformers
img: # optional card image, e.g. assets/img/projects/revisit.jpg
importance: 1
category: research
---

**ReVisiT: Revisiting Only What Changed for Efficient Video Vision Transformers** _(manuscript under review)_

Consecutive video frames are mostly redundant, yet vision transformers recompute every token for every frame. ReVisiT uses changes between frames to decide which tokens to recompute and reuses cached activations everywhere else, without any retraining.

#### Method

- Luminance-based change detection selects the tokens that changed between frames.
- One-hop spatial expansion adds the neighbors of changed tokens to the recomputed set.
- Temporal activation caching reuses the stored activations of all other tokens across frames.

#### Results

| Task                      | Model         | Dataset      | Metric  | ReVisiT | Dense  | Backbone ops saved |
| ------------------------- | ------------- | ------------ | ------- | ------- | ------ | ------------------ |
| Video object detection    | ViTDet-B      | ImageNet VID | mAP@0.5 | 82.27%  | 82.37% | 69.3%              |
| Pose estimation           | ViTPose-S/16  | Sub-JHMDB    | PCK@0.2 | 95.77%  | 95.75% | 64.6%              |
| Video object segmentation | DINO ViT-S/16 | DAVIS 2017   | J&F     | 60.64%  | 61.8%  | 33.8%              |

Operation savings are estimated backbone operations relative to dense inference.

#### Baselines and ablations

- Adapted Eventful Transformers and STC-Cacher for pose estimation and segmentation, and MaskVD for segmentation.
- Ablations on spatial expansion, periodic refresh, and attention update strategies characterize the accuracy–computation tradeoff.
