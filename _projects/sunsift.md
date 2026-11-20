---
layout: page
title: SunSift
description: Battery-free computer vision on solar-powered microcontrollers (IEEE ACSOS 2025)
img: # optional card image, e.g. assets/img/projects/sunsift.jpg
importance: 5
category: research
github: https://github.com/shayangerami/SunSift
related_publications: true
---

**SunSift: Solar-Powered Intelligent Sensing Through Informative Sample Selection** {% cite gerami2025sunsift %}

SunSift runs sample selection and lightweight vision inference on a solar-powered microcontroller, so a battery-free sensor spends its limited energy only on informative samples. I presented this work in the Poster & Demo Track at IEEE ACSOS 2025 in Tokyo, Japan.

#### Highlights

- Built a battery-free vision pipeline that selects informative samples and runs lightweight CNN inference on microcontrollers using TensorFlow Lite Micro.
- Converted the PyTorch-trained sampler through ONNX and TensorFlow Lite for microcontroller deployment.
- Designed selective MRAM checkpointing and implemented a six-state voltage-aware controller for sensing, computing, loading, storing, sleeping, and transmitting.

Code: [github.com/shayangerami/SunSift](https://github.com/shayangerami/SunSift)
