---
layout: page
title: SCENE
description: Sparse event-driven video reconstruction for frame-based object detection
img: # optional card image, e.g. assets/img/projects/scene.jpg
importance: 3
category: research
---

**SCENE: A Sparse Capacitive Event-Driven Near-Sensor Engine for Frame-Compatible Object Detection** _(manuscript under review)_

SCENE is a sparse, event-driven in-sensor and near-sensor engine that reconstructs conventional video frames from selected changes, so existing frame-based object detectors can process them. I built the system-level evaluation.

#### Evaluation

- Evaluated reconstruction on 30,402 ImageNet-VidVRD frames across 107 videos, compared against full-frame processing, running-average background modeling, and ViBe.
- Swept comparison thresholds, resolutions, and periodic full-frame refresh schedules, measuring image fidelity, modeled data transfer, and detector accuracy.
- Integrated YOLOV++ inference and fine-tuning on reconstructed frames.

#### Results

- One configuration reached 83% mAP@0.5 with 56% lower modeled data transfer than full-frame processing.
- Another reached 82% mAP@0.5 at 0.80 MB/frame of modeled transfer, versus 2.76 MB/frame for full frames.
